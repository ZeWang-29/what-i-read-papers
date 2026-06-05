# Steyvers et al. (2025) — What large language models know and what people think they know

**Nature Machine Intelligence 2025**

---

## Overview

- **Paper type**: Empirical (behavioral experiments with human participants)
- **Central claim**: There is a significant gap between what LLMs internally "know" (their calibration and discrimination ability) and what humans perceive based on LLM-generated explanations. This gap can be reduced by aligning explanation style with model confidence.
- **Number of evidence blocks**: 4
- **Evidence block purposes**:
  1. Experiment 1 — Measure the calibration and discrimination gap using default LLM explanations
  2. Experiment 2 — Manipulate uncertainty language and explanation length to see how they affect human confidence
  3. Alignment analysis — Show that matching explanation style to model confidence reduces both gaps
  4. Explanation length effect — Longer explanations increase human confidence without improving discrimination
- **Block relationships**: Block 1 establishes the problem (gaps exist) → Block 2 shows what levers affect human confidence → Block 3 uses those levers to fix the problem → Block 4 identifies a specific pitfall (length bias)
- **Key concepts**:
  - **Calibration gap**: difference between how well model confidence vs. human confidence tracks actual accuracy
  - **Discrimination gap**: difference between how well model vs. humans can distinguish correct from incorrect answers
- **Conclusion**: Default LLM explanations mislead users into overconfidence. By adding uncertainty language ("I am not sure" / "I am somewhat sure" / "I am sure") aligned with the model's internal confidence, both the calibration and discrimination gaps can be substantially reduced.

---

### High-Level Summary

LLMs are internally reasonably well calibrated — their token probabilities track answer accuracy. But users never see these probabilities. Instead, they see confident-sounding text explanations that don't reflect the model's actual uncertainty. This paper shows that humans systematically overestimate LLM accuracy when reading default explanations, and that longer explanations make this worse (more confidence without more accuracy). The fix is simple: prepend uncertainty language (like "I am not sure") matched to the model's internal confidence score. This significantly narrows the gap between what the model knows and what the user thinks it knows.

---

## Block 1: Experiment 1 — The Calibration and Discrimination Gap

### Participants and Design (in plain words)

Three sub-experiments, each with a different LLM and question type:

| Experiment | LLM | Question type | Dataset | N participants |
|---|---|---|---|---|
| 1a | GPT-3.5 | Multiple choice | MMLU | 41 |
| 1b | PaLM2 | Multiple choice | MMLU | 39 |
| 1c | GPT-4o | Short answer | TriviaQA | 42 |

Participants (recruited online) see a question, the LLM's answer, and the LLM's default explanation. They then judge: "What is the probability that the LLM's answer is correct?" They do NOT see the model's internal confidence score.

### What is model confidence?

For multiple-choice: the token probability assigned to the selected answer (e.g., 0.46 for option C). For short answer: an additional prompting step where the LLM evaluates whether its own answer is true or false, and the probability of "true" is used.

### Metrics

- **ECE (Expected Calibration Error)**: how well confidence tracks accuracy. Lower = better.
- **AUC (Area Under the Curve)**: how well confidence discriminates between correct and incorrect answers. Higher = better.

### Results

**Calibration gap**: Model ECE is much lower than human ECE across all three LLMs. Humans are systematically overconfident — they think the LLM is more accurate than it actually is.

**Discrimination gap**: Models discriminate well between correct and incorrect answers (AUC 0.746–0.781). Humans reading default explanations do barely better than random guessing (AUC 0.589–0.602).

### What this means

Default LLM explanations are misleading. They sound confident regardless of whether the answer is right or wrong. The model internally "knows" when it's uncertain, but this uncertainty is not conveyed in the text.

---

## Block 2: Experiment 2 — Manipulating Uncertainty Language and Length

### Design (in plain words)

Same setup as experiment 1, but now the LLM explanations are systematically manipulated along two dimensions:

- **Uncertainty language** (3 levels): "I am not sure" / "I am somewhat sure" / "I am sure"
- **Explanation length** (3 levels): long / short / uncertainty statement only

This creates 3 × 3 = 9 explanation types per question. Each participant sees a random assignment.

| Experiment | LLM | N participants |
|---|---|---|
| 2a | GPT-3.5 (multiple choice) | 60 |
| 2b | PaLM2 (multiple choice) | 60 |
| 2c | GPT-4o (short answer) | 59 |

### Results

**Uncertainty language works**: "Not sure" → significantly lower human confidence. "Sure" → significantly higher. BF > 100 across all experiments.

**Length increases confidence**: Longer explanations → higher human confidence (BF = 25). But longer explanations do NOT improve discrimination (AUC 0.54 for long vs. 0.57 for uncertainty-only). So length inflates confidence without adding useful information.

### What this means

Two levers exist: uncertainty language (helpful — changes confidence in the right direction) and length (harmful — increases confidence without improving accuracy judgment). Users interpret length as a signal of confidence/quality, even though it isn't.

---

## Block 3: Reducing the Gaps — Aligning Explanation Style with Model Confidence

### Method (in plain words)

Simple decision rule: based on the model's internal confidence score, select which explanation style to show the user:

- Model confidence low → show "I am not sure" explanation
- Model confidence medium → show "I am somewhat sure" explanation
- Model confidence high → show "I am sure" explanation

Two threshold parameters determine the cutoffs. The researchers simulate this by filtering experiment 2 data: for each question, only keep the human confidence ratings from participants who happened to see the explanation style that matches the model's confidence level.

### Results

Both gaps narrow substantially:

- **Calibration gap**: human ECE decreases for all three LLMs, moving closer to model ECE
- **Discrimination gap**: human AUC increases significantly (BF > 100 for experiments 2a and 2c, BF = 6.48 for 2b)

### What this means

A simple intervention — prepending uncertainty language matched to the model's internal confidence — significantly improves how well users can judge LLM accuracy. The model's internal self-knowledge CAN be communicated to users, it just isn't in current default settings.

---

## Block 4: The Length Bias Problem

### Finding

Across all experiments, longer explanations increase human confidence without improving their ability to distinguish correct from incorrect answers. This is a systematic bias: users treat length as a proxy for quality/confidence.

### Why this matters

Current LLMs tend to generate verbose explanations by default. This verbosity makes users MORE confident in LLM answers, even when the LLM is wrong. This is the opposite of what good uncertainty communication should do.

### Implication for design

LLM interfaces should not just be verbose and confident-sounding. Shorter, calibrated explanations with explicit uncertainty language would serve users better than long, detailed but uncalibrated explanations.

---

## Counter-arguments & Limitations

| Issue | Paper's response |
|---|---|
| Participants lack domain knowledge, so they can't independently judge | This is intentional — mirrors real use cases where people consult LLMs precisely because they lack expertise. Participant accuracy (45-51%) closely matched LLM accuracy. |
| The selection rule is simulated, not tested in a real deployment | Acknowledged — the filtering approach approximates but doesn't directly test a live system |
| Only three LLMs tested | GPT-3.5, PaLM2, GPT-4o cover different architectures, and results are consistent across all three |
| Threshold parameters for the decision rule might be overfit | Supplementary analysis shows results are not sensitive to parameter settings |

---

## Open Questions

**Flagged by the paper:**
- How do these findings extend to more complex, open-ended tasks (not just Q&A)?
- Can LLMs learn to self-calibrate their explanations without external intervention?
- How does explanation style interact with user expertise?

**My questions:**
- (Add your own questions here after reading)
