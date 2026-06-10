# Azrieli, Chambers & Healy (2018) — Incentives in Experiments: A Theoretical Analysis

**Journal of Political Economy 2018, Vol 126, No. 4: 1472–1503**

---

## Overview

### Blocks

This paper has **4 blocks**:

1. **Theory Block 1 — Framework + Proposition 0**: Sets up the general framework (choice objects X, payment objects P(X), mechanisms, incentive compatibility) and proves that no mechanism is incentive compatible without assumptions
2. **Theory Block 2 — Monotonicity + RPS mechanism (Proposition 1, Theorem 1)**: Proves that under statewise monotonicity, Random Problem Selection (pay for one randomly chosen task) is essentially the only incentive compatible mechanism
3. **Theory Block 3 — NCaT + Pay-All mechanism (Proposition 2, Theorem 2)**: Proves that under "no complementarities at the top," paying for every task is essentially the only incentive compatible mechanism
4. **Empirical Block — Survey + existing evidence**: Reviews how experimenters actually pay subjects and surveys empirical tests of monotonicity and NCaT

### Block Relationships

- Block 1 establishes that assumptions are necessary (you can't avoid them)
- Blocks 2 and 3 give two parallel paths: different assumptions → different mechanisms
- Block 4 helps experimenters decide which assumption (and thus which mechanism) is appropriate for their setting

### Research Question

When an experiment has multiple tasks, how should subjects be paid? Which payment mechanism is incentive compatible under which assumptions?

### Conclusion

There are exactly two defensible payment mechanisms: (1) Random Problem Selection (pay one random task) — justified by monotonicity, and (2) Pay-All (pay every task) — justified by no complementarities at the top. The experimenter must choose based on which assumption is more plausible in their setting. Most published papers do not justify their choice.

---

### High-Level Summary

This paper solves a foundational problem in experimental economics: how to pay subjects when they make multiple decisions. The key insight is the distinction between choice objects X (what subjects choose among) and payment objects P(X) (what subjects actually receive). Under RPS, subjects choose among lotteries but receive compound lotteries; under Pay-All, subjects choose individual items but receive bundles. Incentive compatibility depends on preferences over P(X), but experimenters design experiments to learn about preferences over X — and their theories rarely extend to P(X). The paper proves that under a minimal assumption (monotonicity), RPS is essentially the unique IC mechanism, and under a different minimal assumption (NCaT), Pay-All is essentially the unique IC mechanism. This gives experimenters a clean framework: pick the assumption that fits your setting, and the mechanism follows.

---

## Block 1: Framework + Proposition 0

### Setup (in plain words)

An experiment asks a subject to make decisions in k separate tasks (e.g., choose a lottery in task 1, choose a lottery in task 2, etc.). The experimenter needs a payment mechanism — a rule that maps the subject's announced choices into actual payments.

The critical distinction:
- **X** = the set of choice objects (what subjects choose from in each task)
- **P(X)** = the set of payment objects (what subjects actually receive)

These are NOT the same. Example: if subjects choose among simple lotteries and you use RPS (pay one random task), then X = simple lotteries, but P(X) = compound lotteries (because the randomization over which task gets paid creates an extra layer of randomness). Subjects announce choices over X but actually receive objects in P(X).

**Incentive compatibility** = the subject always does best by choosing truthfully (their genuine favorite) in every task, regardless of their preferences.

### Proposition 0

If you make NO assumptions about how subjects evaluate objects in P(X), then no mechanism is incentive compatible when there are multiple tasks.

### What this means (in plain words)

You can't avoid making assumptions. Every payment mechanism requires SOME assumption about how subjects evaluate the payments they receive. The question is: which assumption is weakest and most defensible?

### Survey finding

The authors surveyed all experimental papers in the top-5 economics journals and Experimental Economics in 2011. Of papers with multiple tasks: 29% don't even describe which mechanism they used, 48% describe it but don't justify it, only 23% explicitly justify their choice. And in ZERO papers did the theory extend to P(X), meaning incentive compatibility couldn't be formally evaluated.

---

## Block 2: Monotonicity + RPS Mechanism

### The assumption: Statewise Monotonicity (in plain words)

If act A gives you something at least as good as act B in every possible state of the world, and strictly better in at least one state, then you prefer A to B.

This is extremely weak — it just says you prefer to get better stuff. It allows for wealth effects, portfolio effects, hedging, and any preference model (not just expected utility).

### Proposition 1

If all admissible extensions satisfy monotonicity, then the RPS mechanism is incentive compatible.

### Why (in plain words)

Under RPS, one task is randomly chosen for payment. If you lie in task i (choose something you don't actually prefer), the only thing that changes is: in the state where task i is selected for payment, you get something worse. In all other states, nothing changes. So lying is dominated by truth-telling. Monotonicity guarantees that a dominated act is never preferred.

### Theorem 1

Under monotonicity (and nothing else), RPS is essentially the **only** incentive compatible mechanism.

### The reduction trap (in plain words)

Previous papers (Holt 1986, Karni & Safra 1987) showed cases where RPS is NOT incentive compatible. How does this square with Proposition 1?

The answer: those papers assumed **reduction of compound lotteries** — that subjects simplify compound lotteries into simple ones. Reduction + monotonicity together imply expected utility (independence axiom). So the problem isn't with RPS; it's that reduction is a strong assumption. Without reduction, monotonicity alone is enough, and no structure on preferences over X is required.

Takeaway for experimenters: if you use RPS, you should think about whether your subjects might reduce compound lotteries. If they present all tasks on one screen (making the compound structure salient), reduction is more likely. If tasks are on separate screens, reduction is less likely, and monotonicity is more defensible.

---

## Block 3: NCaT + Pay-All Mechanism

### The assumption: No Complementarities at the Top (NCaT, in plain words)

Take the subject's favorite item from each task and bundle them together. NCaT says: this bundle of favorites must be the subject's most preferred bundle overall. No complementarity between items is strong enough to make a non-favorite bundle better than the all-favorites bundle.

Example of a violation: subject prefers lottery A in task 1 and lottery C in task 2, but A and C together create too much risk, so they'd rather have the "worse" B and D which hedge each other.

NCaT says this doesn't happen (at the top).

### Proposition 2

If all admissible extensions satisfy NCaT, then the Pay-All mechanism is incentive compatible.

### Theorem 2

Under NCaT (and nothing else), Pay-All is essentially the **only** incentive compatible mechanism.

### When NCaT might fail (in plain words)

- Portfolio effects: choosing riskier lotteries in each task because the diversification across tasks reduces total risk
- Wealth effects: winnings from early tasks change risk preferences in later tasks
- Hedging: deliberately choosing a bad option in one task to hedge against risk in another

---

## Block 4: Empirical Evidence

### What this block does

Theory tells you WHICH assumption you need, but not WHETHER it holds in your setting. That's an empirical question.

### Testing monotonicity (summary of existing evidence)

Between-subjects design: one group does the full experiment with RPS, another group does only one task (where IC is trivial). Compare choices.

- Starmer & Sugden (1991): mostly no violations (p = .223 and p = .052)
- Cubitt et al. (1998): no violations (p = .685 and p = .120)
- Brown & Healy (2018): violation when all tasks shown on one screen (p = .040), but NOT when tasks shown on separate screens (p = .697)
- Camerer (1989): less than 3% of subjects wanted to change their decision after the payment state was revealed

Key finding: monotonicity violations are linked to **how tasks are presented**. Separate screens → monotonicity holds. One screen → subjects may reduce compound lotteries, causing violations.

### Testing NCaT

Less directly tested, but portfolio effects and wealth effects have been documented in some settings, suggesting NCaT can fail when tasks involve correlated risks.

### Practical advice for experimenters

1. Decide whether monotonicity or NCaT is more plausible in your setting
2. If using RPS: present tasks on separate screens, avoid making compound structure salient
3. If using Pay-All: be cautious of portfolio effects and wealth effects
4. You can run your own between-subjects test to check

---

## Counter-arguments & Key Distinctions

| Concern | Paper's response |
|---|---|
| "RPS requires expected utility" (Holt 1986, Karni & Safra 1987) | Only if you also assume reduction. Without reduction, monotonicity alone is enough — no preference structure on X required |
| "Pay-All creates portfolio effects" | Yes, which is why it requires NCaT. If portfolio effects are a concern, use RPS instead |
| "Can you test these assumptions?" | Yes, between-subjects design. But there's a regress problem (the test itself needs an IC mechanism). Practical solutions exist |
| "What about games?" | Same framework applies. With no feedback between games, RPS works. With feedback or repeated games against same opponent, treat the whole thing as one decision problem |
