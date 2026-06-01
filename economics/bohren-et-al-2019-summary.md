# Bohren, Imas & Rosenberg (2019) — The Dynamics of Discrimination: Theory and Evidence

**AER 2019, 109(10): 3395–3436**

---

## Overview

### Blocks

This paper has **6 blocks**:

1. **Theory Block 1 — Model Setup + Proposition 1 (Subjectivity of Judgment)**: Establishes the model and shows that varying the objectivity of quality signals can distinguish belief-based from preference-based discrimination.
2. **Theory Block 2 — Proposition 2 (Impossibility of Reversal)**: Shows that with correct beliefs and common knowledge, discrimination mitigates over time but never reverses.
3. **Theory Block 3 — Proposition 3 (Possibility of Reversal)**: Shows that with heterogeneous evaluators (some biased, some aware of bias), discrimination can reverse.
4. **Experiment Block 1 — Field Experiment on Online Math Forum (Questions & Answers)**: Tests whether subjectivity affects discrimination (answers = objective, questions = subjective).
5. **Experiment Block 2 — Field Experiment: Dynamics (Novice vs Advanced)**: Tests whether discrimination reverses when women have established track records.
6. **Observational Block — Forum Data Analysis**: Uses observational data to rule out alternative explanations (attrition, variance differences, autocorrelation) and replicate experimental findings.

### Block Relationships

- Blocks 1–3 (theory) generate testable predictions that differ by source of discrimination
- Block 4 (experiment: subjectivity) tests Proposition 1 → distinguishes belief-based vs. preference-based
- Block 5 (experiment: dynamics) tests Propositions 2 & 3 → distinguishes correct beliefs vs. biased beliefs
- Block 6 (observational) provides robustness and rules out confounds for Block 5's reversal finding

### Research Questions

1. How does discrimination evolve dynamically (over time with accumulating track records)?
2. Can this dynamic evolution identify the **source** of discrimination (correct beliefs vs. biased beliefs vs. preferences)?

### Conclusion

Discrimination on the forum is driven by **biased beliefs** (incorrect stereotypes), not preferences or correct statistical discrimination. Evidence: (i) discrimination disappears when judgment is objective (answers), ruling out preferences; (ii) discrimination reverses for established users, ruling out correct beliefs and pointing to biased beliefs with misspecification.

---

## Block 1: Theory — Model Setup + Proposition 1 (Subjectivity)

### Assumptions

- Worker has group identity $g \in \{M, F\}$ and unobservable ability $a \sim N(\mu_g, 1/\tau_a)$
- Worker completes tasks with quality $q_t = a + \varepsilon_t$, where $\varepsilon_t \sim N(0, 1/\tau_\varepsilon)$
- Evaluator observes signal $s_t = q_t + \eta_t$, where $\eta_t \sim N(0, 1/\tau_\eta)$
  - $\tau_\eta$ captures **subjectivity of judgment**: lower $\tau_\eta$ = more subjective
- Evaluator has type $\theta_i$ determining:
  - Subjective belief about average ability by gender: $\hat{\mu}_g$ (may differ from true $\mu_g$)
  - Taste parameter $c_F$ (disamenity from evaluating female workers)
  - Subjective belief about other evaluators' type distribution: $\hat{\pi}_i$
- Evaluator maximizes payoff: $-(v - (q - c_g))^2$, so optimal evaluation $= E[q \mid h, s, g] - c_g$

### Key Definitions

- **Belief-based partiality**: $\hat{\mu}_M > \hat{\mu}_F$ (believes men have higher average ability)
  - Unbiased if $\hat{\mu}_g = \mu_g$; biased otherwise
- **Preference-based partiality**: $c_F > 0$ (taste against women)
- **Discrimination**: $D(h, s) = v(M, h, s) - v(F, h, s) > 0$ (men get higher evaluations for same history and signal)

### Key Formula — Initial Discrimination (Eq. 5)

$$D(h_1, s_1) = \frac{\tau_q}{\tau_q + \tau_\eta} (\hat{\mu}_M - \hat{\mu}_F) + c_F$$

where $\tau_q = \frac{\tau_a \cdot \tau_\varepsilon}{\tau_a + \tau_\varepsilon}$ is the precision of the prior on quality.

### Proposition 1 (Subjectivity of Judgment)

- If belief-based partiality: initial discrimination is **decreasing** in $\tau_\eta$ (more objective → less discrimination)
- If preference-based partiality: initial discrimination is **constant** w.r.t. $\tau_\eta$
- In the limit $\tau_\eta \to \infty$ (perfectly objective): discrimination exists iff preference-based partiality exists

### Detailed Derivation of Eq. 5

**Step 1: Prior distribution of quality.** Since $q_1 = a + \varepsilon_1$ with $a \sim N(\hat{\mu}_g, 1/\tau_a)$ and $\varepsilon_1 \sim N(0, 1/\tau_\varepsilon)$ independent, the sum of two independent normals gives:

$$q_1 \sim N\left(\hat{\mu}_g, \; \frac{1}{\tau_a} + \frac{1}{\tau_\varepsilon}\right)$$

The precision of this prior is $\tau_q = \frac{\tau_a \cdot \tau_\varepsilon}{\tau_a + \tau_\varepsilon}$.

**Step 2: Posterior after observing signal.** The signal is $s_1 = q_1 + \eta_1$ where $\eta_1 \sim N(0, 1/\tau_\eta)$. This is standard Normal-Normal Bayesian updating (prior precision $\tau_q$, signal precision $\tau_\eta$), giving a precision-weighted average of prior mean and signal:

$$E[q_1 \mid s_1, g] = \frac{\tau_q \cdot \hat{\mu}_g + \tau_\eta \cdot s_1}{\tau_q + \tau_\eta}$$

**Step 3: Optimal evaluation.** From the quadratic loss $-(v - (q - c_g))^2$, the optimal evaluation is the posterior mean minus the taste parameter:

$$v^*(g, h_1, s_1) = \frac{\tau_q \cdot \hat{\mu}_g + \tau_\eta \cdot s_1}{\tau_q + \tau_\eta} - c_g$$

**Step 4: Discrimination.** Taking the difference $D = v^*(M) - v^*(F)$:

$$D = \frac{\tau_q \hat{\mu}_M + \tau_\eta s_1}{\tau_q + \tau_\eta} - c_M - \frac{\tau_q \hat{\mu}_F + \tau_\eta s_1}{\tau_q + \tau_\eta} + c_F$$

The $s_1$ terms cancel (same signal for both genders), and $c_M = 0$ (normalized), yielding Eq. 5:

$$D(h_1, s_1) = \frac{\tau_q}{\tau_q + \tau_\eta}(\hat{\mu}_M - \hat{\mu}_F) + c_F$$

**Note on originality:** The Normal-Normal updating framework is standard (Phelps 1972, Aigner & Cain 1977). The social psychology literature (Fiske et al. 1991) already observed that subjectivity increases stereotype reliance. This paper's contribution is formalizing $\tau_\eta$ as an **identification tool** — using variation in signal precision to distinguish belief-based from preference-based discrimination — and extending the framework dynamically.

### Derivation (high-level)

From Eq. 5: the belief-based component is weighted by $\frac{\tau_q}{\tau_q + \tau_\eta}$. As $\tau_\eta$ increases (more precise signal), this weight shrinks → belief about group differences matters less. The preference component $c_F$ is additive and independent of $\tau_\eta$.

### Intuition

When you can perfectly observe quality (e.g., a math answer is correct or not), it doesn't matter what your prior beliefs about group ability are — you see the truth directly. But when quality is hard to judge (e.g., "is this question interesting?"), you lean more on stereotypes/priors about the group. Preferences, however, are a fixed "tax" on women regardless of how clearly you see quality.

---

## Block 2: Theory — Proposition 2 (Impossibility of Reversal)

### Assumptions

- Single evaluator type with common knowledge of shared beliefs
- Belief-based partiality ($\hat{\mu}_M > \hat{\mu}_F$), no preference-based partiality ($c_F = 0$)
- Evaluators correctly model that all others share the same beliefs

### Key Mechanism

After period 1, a female who received evaluation $v$ must have produced a higher signal than a male with the same evaluation (from Eq. 6):

$$s(v, \hat{\mu}_g) = \frac{\tau_q + \tau_\eta}{\tau_\eta} \cdot v - \frac{\tau_q}{\tau_\eta} \cdot \hat{\mu}_g$$

Since $\hat{\mu}_F < \hat{\mu}_M$, we get $s(v, \hat{\mu}_F) > s(v, \hat{\mu}_M)$. So evaluators know the female's evaluation is a stronger signal of ability.

### Proposition 2 (Impossibility of Reversal)

With a single type of evaluator with belief-based partiality and no preference-based partiality: fixing an evaluation history, **discrimination decreases across periods but never reverses**.

### Derivation (high-level)

The posterior mean of ability is increasing in the prior mean. Two opposing effects: (i) higher prior mean directly raises posterior (MLRP of prior); (ii) higher prior mean means a lower signal was required to receive the evaluation (MLRP of signal distribution, decreasing in prior mean). The proof shows effect (i) dominates: if you start with $\hat{\mu}_M > \hat{\mu}_F$, then posterior mean for male > posterior mean for female after any common evaluation history. Beliefs converge but never cross.

### Intuition

Even though evaluators know the female had to clear a higher bar, the original prior advantage for males still dominates the update. Think of it as: the prior gets diluted by new evidence but never fully overwhelmed when everyone agrees on the same model. The gap shrinks but the ordering is preserved.

---

## Block 3: Theory — Proposition 3 (Possibility of Reversal)

### Assumptions

- Two types of evaluators:
  - **Heuristic type ($\theta_1$)** with probability $p$: has biased belief-based partiality ($\hat{\mu}_M^1 > \hat{\mu}_F^1$), unaware of bias, believes all others are the same type (bias blind spot / false consensus)
  - **Impartial type ($\theta_2$)** with probability $1-p$: no belief-based partiality ($\hat{\mu}_M^2 = \hat{\mu}_F^2$), aware that heuristic types exist, correctly estimates their prevalence ($\hat{\pi}_2(\theta_1) = p$)
- Both types agree on average male ability: $\hat{\mu}_M^1 = \hat{\mu}_M^2 = \hat{\mu}_M$
- No preference-based partiality

### Key Formula — Initial Aggregate Discrimination (Eq. 7)

$$D(h_1, s_1) = p \cdot \frac{\tau_q}{\tau_q + \tau_\eta} (\hat{\mu}_M - \hat{\mu}_F^1) > 0$$

Only heuristic types contribute to initial discrimination.

### Proposition 3 (Possibility of Reversal)

For any initial evaluation $v_1$ (or any second-period signal $s_2$), there exist cutoffs $\bar{p}$ such that for a low enough share of heuristic types ($p \in (0, \bar{p})$) and a high enough signal (or low enough first evaluation), **aggregate discrimination reverses in the second period**: $D(v_1, s_2) < 0$.

### Derivation (high-level)

After period 1:
- Heuristic type: still discriminates against females (by Prop. 2, beliefs don't reverse within a single-type model)
- Impartial type: knows the female likely faced a biased evaluator → the evaluation is an even stronger signal of her ability → posterior **favors** females ($\hat{\mu}_F^2(v_1) > \hat{\mu}_M^2(v_1)$)

Aggregate 2nd-period discrimination = weighted average. Non-monotonic in $p$:
- $p = 0$: no discrimination (all impartial)
- $p = 1$: positive discrimination against females (all heuristic, never reverses)
- Low $p$: few heuristic evaluators, but impartial types strongly favor females → reversal possible

### Intuition

If you're a sophisticated evaluator who knows that some evaluators are sexist, and you see a woman with a strong track record, you infer: "she must be *really* good to have overcome biased evaluation." This makes you favor her over a man with the same track record. When there are enough sophisticated evaluators relative to biased ones, this "she must be even better" effect dominates at the aggregate level, and discrimination flips.

---

## Block 4: Experiment — Subjectivity (Questions vs. Answers)

### Participants / Platform

- Platform: a large online math Q&A forum (Stack Exchange family; ~350K users, 3.5M questions/year, 4.3M answers/year)
- Evaluators: regular forum users who vote on posts (anonymous voting)
- Not a paid lab experiment — the evaluators are organic platform users who encounter the experimental posts naturally
- No payment to evaluators; this is a field experiment embedded in normal platform activity

### Design

- Created **140 Novice accounts** (70 male usernames, 70 female usernames) for posting **answers**
- Answers written by research assistants in pairs: "answerer" writes answer without knowing which account it will be posted to; "poster" assigns to predetermined account (double-blind for content quality)
- Posted original correct math answers to newly posted questions
- Also posted **questions** from 140 Novice accounts (70 male, 70 female) — see Block 5 for full design
- Questions: judgment criteria are **subjective** (interesting? well-researched? novel?)
- Answers: judgment criteria are **objective** (correct or not?)
- Data collected 7 days after posting; 5 of 140 answers dropped due to errors

### What This Captures

Tests Proposition 1: if discrimination is belief-based, it should be mitigated when judgment is more objective (answers). If preference-based, discrimination should be the same for questions and answers.

### Results

**Regressions (Table 1):**

1. $\Delta \text{Rep}$ (answers) on Male dummy: coefficient $= -1.38$ (SE $= 0.97$), **not significant** → no gender discrimination on answers
2. Net votes (answers) on Male dummy: coefficient $= -0.31$ (SE $= 0.17$), **not significant**
3. $\Delta \text{Rep}$ (questions, novice) on Male dummy: coefficient $= 2.86$ (SE $= 1.32$), **significant** → males earn ~2.86 more reputation points per question
4. Net votes (questions, novice) on Male dummy: coefficient $= 0.58$ (SE $= 0.27$), **significant** → males get ~0.58 more net votes per question
5. Pooled (questions + answers): Male $\times$ Question interaction for $\Delta \text{Rep} = 4.24$ (SE $= 1.64$), **significant**
6. Pooled: Male $\times$ Question interaction for net votes $= 0.89$ (SE $= 0.32$), **significant**

**Interpretation:**
- No discrimination on answers (objective judgment)
- Significant discrimination against females on questions (subjective judgment)
- The difference between questions and answers is statistically significant (interaction term)
- Effect size for questions: ~0.4 standard deviations

**Conclusion:** Consistent with belief-based partiality (Proposition 1), **inconsistent** with preference-based partiality.

---

## Block 5: Experiment — Dynamics (Novice vs. Advanced)

### Design

- **280 accounts** total for questions: 140 Novice (70M, 70F) + 140 Advanced (70M, 70F)
- **Advanced accounts**: Research assistants manually built reputation to top 25th percentile ($\geq 100$ points; mean $= 155.23$) by posting content
- **Critical**: After reaching high reputation, **re-randomized gender** of Advanced usernames (35 male→female, 35 female→male, 70 same gender new name). All past activity displays new username. No public record of name change.
- This ensures informational content of reputation is **identical** across genders for Advanced accounts (mean rep: female $154.57$ vs male $155.89$, $p = 0.82$)
- Posted 280 original math questions (upper-undergrad to early-grad level), randomly assigned to 4 conditions: male novice, female novice, male advanced, female advanced
- Posting schedule: 1 question every 20+ min, 5pm–10pm, Mon–Thu
- Data collected 7 days after posting; 7 of 280 dropped
- Usernames from SSA "Top Names of the 2000s" list

### What This Captures

Tests Propositions 2 & 3: if discrimination against novice women reverses for advanced women (same questions, only reputation differs), this rules out correct beliefs (Prop 2 says no reversal) and points to biased beliefs with misspecification (Prop 3 says reversal possible).

### Results

**Regressions (Table 2):**

*Advanced accounts only:*
1. $\Delta \text{Rep}$ on Male dummy: coefficient $= -3.16$ (SE $= 1.37$), **significant** → advanced females earn MORE reputation than males
2. Net votes on Male dummy: coefficient $= -0.62$ (SE $= 0.28$), **significant** → advanced females get more net votes

*Novice + Advanced pooled:*
3. $\Delta \text{Rep}$: Male $= 2.86$ (SE $1.36$), Advanced $= -2.33$ (SE $1.35$), Male $\times$ Advanced $= -6.02$ (SE $1.91$), **significant**
4. Net votes: Male $= 0.58$ (SE $0.27$), Advanced $= -0.49$ (SE $0.27$), Male $\times$ Advanced $= -1.20$ (SE $0.38$), **significant**
5. Binary ($\geq 1$ upvote): Male $= 0.17$ (SE $0.08$), Advanced $= -0.09$ (SE $0.08$), Male $\times$ Advanced $= -0.40$ (SE $0.11$), **significant**

*Chi-squared tests for difference between Novice and Advanced male coefficients:*
- $\Delta \text{Rep}$: $\chi^2(1) = 9.88$, $p = 0.002$
- Net votes: $\chi^2(1) = 10.05$, $p = 0.002$

**Interpretation:**
- Novice: males favored (~0.4 SD advantage)
- Advanced: females favored (~0.6 SD advantage)
- The **reversal** is statistically significant (interaction term and chi-squared tests)
- Results robust to binary specification (rules out herding/outliers)
- No significant difference in pooled (across gender) evaluations between Novice and Advanced accounts (consistent with shifting standards)

**Conclusion:** Dynamic reversal observed → rules out correct beliefs (Prop 2), consistent with biased beliefs model (Prop 3). Discrimination is driven by belief-based partiality with misspecification.

---

## Block 6: Observational Data — Robustness and Alternative Explanations

### Data

- Forum's publicly available observational dataset: 315,792 users, July 2010 – March 2017
- Gender inferred from usernames using Vasilescu, Capiluppi & Serebrenik (2014) algorithm
- 55% of accounts resolved; of these, 19% female, 81% male
- Among accounts with $<100$ rep: 21% female; accounts with 100–240 rep (Advanced range): 13% female
- Proprietary dataset from the forum: identifies specific users who voted on experimental posts + their historical activity

### Analyses and Results

**1. Attrition (rules out differential exit by gender):**
- Probit: $\Pr(\text{generate next post})$ on gender, $\log(\text{reputation earned on prior post})$, interaction
- Gender and interaction terms **not significant** for any transition (1st→2nd, 2nd→3rd, ..., pooled)
- Conclusion: no differential attrition → reversal not driven by selection

**2. Variance of ability (rules out different variance by gender):**
- Levene's test on distributions of $\Delta \text{Rep}$ for first answer posts by gender
- $p = 0.41$ (mean), $p = 0.48$ (median), $p = 0.46$ (trimmed mean) → **not significant**
- Conclusion: no gender difference in ability variance

**3. Autocorrelation (rules out negative autocorrelation in quality):**
- Wooldridge test for serial correlation in panel data
- Random effects regression of reputation earned on gender dummy, then test residuals
- No significant autocorrelation found for either questions or answers
- Conclusion: reversal not due to mean reversion in quality

**4. Replication with observational data:**
- Regressions analogous to Tables 1 & 2 using $\Delta \text{Rep}$ as dependent variable on full observational sample
- Three main findings mirror experiment:
  - (i) No significant gender discrimination on answers
  - (ii) Novice female questions earn less reputation than novice male questions
  - (iii) Advanced female questions earn more reputation than advanced male questions
- Caveats: cannot control for quality of questions; potential selection between novice and advanced

**5. Robustness with proprietary voting data:**
- Restricted to first vote from each evaluator (excludes repeat votes) → results unchanged
- Checked whether evaluators of questions vs. answers are similar populations: 48% of votes on questions, 52% on answers (SD $= 0.21$) → similar voters evaluate both types
- No significant differences in evaluator characteristics (reputation, gender) across post types

**Overall conclusion:** Alternative explanations (attrition, variance, autocorrelation) are ruled out. Observational data independently replicates the experimental patterns.
