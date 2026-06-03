# Rafailov, Sharma, Mitchell, Ermon, Manning & Finn (2023) — Direct Preference Optimization: Your Language Model Is Secretly a Reward Model

**NeurIPS 2023**

---

## Overview

- **Paper type**: Method paper (new training algorithm)
- **Core contribution**: DPO — a simple classification loss that directly optimizes a language model from human preferences, without needing a separate reward model or RL
- **Problem**: RLHF (Reinforcement Learning from Human Feedback) is the standard way to align LMs with human preferences, but it's complex and unstable: train reward model → run PPO → tune many hyperparameters
- **Key insight**: There exists a closed-form mapping from reward functions to optimal policies. By substituting this mapping into the Bradley-Terry preference model, the reward model and partition function cancel out, leaving a simple binary cross-entropy loss directly on the policy
- **Blocks**:
  1. Method Block 1 — RLHF preliminaries (existing pipeline)
  2. Method Block 2 — DPO derivation (the core contribution)
  3. Method Block 3 — Theoretical analysis (reward model equivalence, instability of actor-critic)
  4. Experiment Block 1 — Controlled sentiment generation (IMDb)
  5. Experiment Block 2 — Summarization (TL;DR) and single-turn dialogue (Anthropic HH)
- **Result summary**: DPO matches or exceeds PPO-based RLHF on all tasks, with much simpler implementation and virtually no hyperparameter tuning

---

### High-Level Summary

The key insight of DPO is a **change of variables**: the standard RLHF objective (maximize reward subject to KL constraint) has a closed-form optimal policy, and this can be rearranged to express the reward as a function of the policy. Substituting this into the Bradley-Terry preference model, the intractable partition function cancels, yielding a simple cross-entropy loss that trains the policy directly. This eliminates the need for a separate reward model, RL training loop, and the instabilities that come with PPO. The result is an algorithm that is dramatically simpler to implement while performing as well or better than RLHF. DPO has become one of the most widely adopted alignment techniques since its publication.

---

## Block 1: Method — RLHF Preliminaries

### Existing Pipeline (3 stages)

**Stage 1: SFT.** Fine-tune a pre-trained LM on high-quality data to obtain $\pi\_{\text{SFT}}$.

**Stage 2: Reward modeling.** Sample response pairs from the SFT model, collect human preference labels (which response is better). Fit a reward model using the Bradley-Terry model:

$$p^{*}(y_1 \succ y_2 \mid x) = \frac{\exp(r^{*}(x, y_1))}{\exp(r^{*}(x, y_1)) + \exp(r^{*}(x, y_2))} = \sigma(r^{*}(x, y_1) - r^{*}(x, y_2))$$

Reward model loss (binary cross-entropy):

$$\mathcal{L}_R(r_\phi, D) = -\mathbb{E}_{(x, y_w, y_l) \sim D} \left[ \log \sigma(r_\phi(x, y_w) - r_\phi(x, y_l)) \right]$$

**Stage 3: RL fine-tuning.** Optimize policy to maximize reward while staying close to reference:

$$\max_{\pi_\theta} \; \mathbb{E}_{x \sim D, \, y \sim \pi_\theta(\cdot|x)} \left[ r_\phi(x, y) \right] - \beta \, D_{\text{KL}} \left[ \pi_\theta(y|x) \| \pi_{\text{ref}}(y|x) \right]$$

where $\beta$ controls the KL penalty and the reference policy is the SFT model.

### Why this is hard

- Must train a separate reward model
- PPO is unstable and requires extensive hyperparameter tuning
- Must sample from the policy during training (expensive)
- Reward model can be exploited (reward hacking)

---

## Block 2: Method — DPO Derivation (Core Contribution)

### Step 1: Closed-form optimal policy

The KL-constrained reward maximization has a known closed-form solution:

$$\pi_r(y \mid x) = \frac{1}{Z(x)} \pi_{\text{ref}}(y \mid x) \exp\left(\frac{1}{\beta} r(x, y)\right)$$

where $Z(x) = \sum_y \pi_{\text{ref}}(y \mid x) \exp\left(\frac{1}{\beta} r(x, y)\right)$ is the partition function.

### Step 2: Rearrange to express reward in terms of policy

Take log of both sides and rearrange:

$$r(x, y) = \beta \log \frac{\pi_r(y \mid x)}{\pi_{\text{ref}}(y \mid x)} + \beta \log Z(x)$$

### Step 3: Substitute into Bradley-Terry and cancel $Z(x)$

The Bradley-Terry model depends only on the **difference** of rewards between two completions. When we substitute the reparameterization, the $\beta \log Z(x)$ terms cancel:

$$p^{*}(y_1 \succ y_2 \mid x) = \sigma\left(\beta \log \frac{\pi^{*}(y_1 \mid x)}{\pi_{\text{ref}}(y_1 \mid x)} - \beta \log \frac{\pi^{*}(y_2 \mid x)}{\pi_{\text{ref}}(y_2 \mid x)}\right)$$

### Step 4: The DPO loss

Replace the optimal policy with a parametric $\pi\_\theta$ and maximize likelihood:

$$\mathcal{L}_{\text{DPO}}(\pi_\theta; \pi_{\text{ref}}) = -\mathbb{E}_{(x, y_w, y_l) \sim D} \left[ \log \sigma\left(\beta \log \frac{\pi_\theta(y_w \mid x)}{\pi_{\text{ref}}(y_w \mid x)} - \beta \log \frac{\pi_\theta(y_l \mid x)}{\pi_{\text{ref}}(y_l \mid x)}\right) \right]$$

### Intuition

The DPO loss does two things simultaneously:
- **Increases** the log probability of preferred completions $y\_w$
- **Decreases** the log probability of dispreferred completions $y\_l$

But it does so with an **adaptive weight**: examples where the implicit reward model incorrectly ranks completions get higher gradient weight. The implicit reward is $\hat{r}\_\theta(x, y) = \beta \log \frac{\pi\_\theta(y|x)}{\pi\_{\text{ref}}(y|x)}$. Without this weighting, the model degenerates (Appendix Table 3).

### Why this is elegant

The entire RLHF pipeline (reward model + PPO + KL constraint) is collapsed into a **single cross-entropy loss**. No sampling from the policy during training. No reward model to maintain. No RL loop. Just supervised learning on preference pairs.

---

## Block 3: Theoretical Analysis

### "Your Language Model Is Secretly a Reward Model"

The implicit reward defined by DPO is:

$$\hat{r}_\theta(x, y) = \beta \log \frac{\pi_\theta(y \mid x)}{\pi_{\text{ref}}(y \mid x)}$$

**Theorem 1**: This reparameterization can represent **all** reward classes consistent with the Bradley-Terry model. No expressiveness is lost.

**Key idea**: Reward functions that differ by only a function of $x$ (not $y$) form an equivalence class — they induce the same preferences and the same optimal policy. The DPO reparameterization simply selects a canonical member from each equivalence class.

### Instability of PPO (actor-critic)

The paper shows that PPO's objective contains a normalization term (the partition function / soft value function) that, if not properly estimated, causes high-variance gradients. PPO handles this with a learned value function (hard to optimize) or a single-sample baseline (noisy). DPO's reparameterization sidesteps this entirely — the partition function cancels analytically.

---

## Block 4: Experiment — Controlled Sentiment Generation (IMDb)

### Task/Dataset

- Prefix: movie review from IMDb dataset
- Goal: generate continuation with positive sentiment
- Preferences generated automatically using a pre-trained sentiment classifier (ground-truth reward available)
- Model: GPT-2-large

### Baselines

PPO (with learned reward), PPO-GT (with ground-truth reward), Unlikelihood, Preferred-FT

### Metrics

Reward-KL frontier: for each algorithm, plot achieved reward vs. KL divergence from reference policy

### Results

- DPO produces the **best reward-KL frontier** — highest reward at every KL level
- DPO **strictly dominates** PPO, even when PPO has access to ground-truth rewards (PPO-GT)
- This is notable: DPO optimizes the same objective as PPO, but more efficiently

### Takeaway

DPO is not just simpler — it's actually a better optimizer of the RLHF objective than PPO itself.

---

## Block 5: Experiments — Summarization & Dialogue

### Summarization (TL;DR)

- **Dataset**: Reddit TL;DR summarization with human preferences (Stiennon et al.)
- **Model**: GPT-J (6B)
- **Evaluation**: GPT-4 win rate vs. human-written reference summaries
- **Results**:
  - DPO: ~61% win rate (temperature 0.0)
  - PPO: ~57% win rate (at its optimal temperature 0.0)
  - DPO is more robust across sampling temperatures
  - Human evaluation: DPO preferred 58% of the time over PPO in head-to-head
- **Out-of-distribution** (CNN/DailyMail): DPO 36% win rate vs. PPO 26% — DPO generalizes better

### Single-turn Dialogue (Anthropic HH)

- **Dataset**: Anthropic Helpful and Harmless (170k dialogues)
- **Model**: Pythia-2.8B
- **Evaluation**: GPT-4 win rate vs. preferred completions in test set
- **Results**:
  - DPO is the **only computationally efficient method** that improves over the preferred completions
  - DPO matches or exceeds Best-of-128 baseline (which requires 128x inference cost)
  - PPO from a public implementation could not beat the base Pythia-2.8B model

### GPT-4 as Evaluator (Human Validation)

- Conducted human study on TL;DR to validate GPT-4 judgments
- GPT-4 agreement with humans is similar to human-human agreement
- GPT-4 (Concise) prompt best approximates human preferences

### Takeaway

DPO scales to real preference datasets and real tasks, matching or exceeding PPO with dramatically less implementation complexity.

---

## Limitations & Future Work

- **Scale**: Only tested up to 6B parameters; behavior at larger scales unknown at time of publication
- **Out-of-distribution**: Initial results are promising but more study needed
- **Reward overoptimization**: Unclear how it manifests in DPO setting
- **Self-labeling**: Can DPO iteratively improve using self-generated preferences (like RLHF with online sampling)?
- **GPT-4 evaluation**: Win rates are sensitive to the evaluation prompt
- **Beyond language**: DPO framework is general — applicable to other generative modalities
