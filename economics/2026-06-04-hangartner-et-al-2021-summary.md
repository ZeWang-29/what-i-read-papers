# Hangartner, Kopp & Siegenthaler (2021) — Monitoring hiring discrimination through online recruitment platforms

**Nature 2021, Vol 589: 572–577**

---

## Overview

### Blocks

This paper has **4 blocks**:

1. **Method Block — Platform data + machine learning approach**: Develops a new methodology to measure hiring discrimination using recruiter click data from an employment website, combined with Lasso-based variable selection to control for all observable jobseeker characteristics
2. **Empirical Block 1 — Ethnic discrimination**: Measures ethnic penalties in contact rates across origin groups
3. **Empirical Block 2 — Time-of-day variation**: Uses within-recruiter variation across the workday to explore drivers of discrimination (implicit bias vs. conscious prejudice)
4. **Empirical Block 3 — Gender discrimination**: Measures gender penalties across 323 occupations, revealing heterogeneity masked by average null effects

### Block Relationships

- Block 1 establishes the identification strategy and validates it
- Blocks 2–4 apply the method to different dimensions of discrimination
- Block 2 (ethnic) is the main result; Block 3 (time-of-day) probes mechanisms; Block 4 (gender) extends the analysis to a second dimension
- Together they demonstrate that the methodology is a general-purpose monitoring tool

### Research Questions

1. Can we use online recruitment platform data to continuously monitor hiring discrimination at scale?
2. How large are ethnic and gender penalties in hiring? What drives them?

### Conclusion

Recruiter click data combined with machine learning can identify hiring discrimination at scale, non-intrusively, and continuously. Ethnic minorities face 4–19% lower contact rates depending on origin. Gender discrimination is occupation-specific: women penalized in male-dominated jobs, men penalized in female-dominated jobs. Time-of-day patterns suggest implicit bias plays a role, as discrimination increases when recruiters are more fatigued.

---

### High-Level Summary

This paper's core contribution is **methodological**: instead of sending fake CVs (correspondence studies, which are expensive, ethically fraught, and limited in scope), they track what real recruiters actually do on a public employment website. The key identification assumption is that the researchers observe the same information as the recruiters — validated by showing that for a subset of recruiters who cannot see names/nationality, estimated ethnic penalties are zero. The Lasso-based post-double selection method controls for 3,729 covariates, making the approach credible at scale. The findings on ethnic hierarchies, time-of-day variation, and occupation-specific gender penalties are empirically rich, but the lasting value of this paper is the monitoring tool itself.

---

## Block 1: Method — Platform Data + Machine Learning Approach

### The setting (in plain words)

The Swiss public employment service runs an online platform where unemployed jobseekers have profiles (entered by case workers, not the jobseekers themselves). Recruiters can search for candidates, view their profiles, and click a "contact button" to request an interview. The researchers tracked everything: who searched for what, which profiles appeared, which profiles were opened, how long recruiters looked at each profile, and whether they clicked the contact button.

### Data

- Period: March to December 2017
- 43,352 recruiters
- 452,729 searches
- 17.4 million profiles appeared in search lists
- 3.4 million profile views
- Outcome: click on the contact button (binary: contacted or not)
- Validated outcome: each click increases probability of leaving unemployment in next 3 months by 2.1% (P < 0.001, n = 12,823,811)

### Identification strategy (in plain words)

The key question is: are ethnic penalties driven by discrimination, or by unobserved differences in productivity?

The approach works because:
1. **Same information**: researchers observe the same CV information that recruiters see
2. **Within-search comparison**: they compare profiles that appeared in the same search (same recruiter, same job criteria), so any search-level factors are held constant
3. **Lasso variable selection**: use post-double selection method (Belloni, Chernozhukov & Hansen 2014) to select which of 3,729 covariates (and first-order interactions) to include — controls for all jobseeker characteristics predictive of either contact or ethnicity

### Validation

For a subset of recruiters who **cannot see** name or nationality (anonymized profiles): regressing contact on ethnicity gives joint F-test P = 0.93 (n = 254,975) — ethnic coefficients are all zero. This confirms that the Lasso-selected controls account for all confounders correlated with ethnicity.

---

## Block 2: Ethnic Discrimination

### Results (in plain words)

Compared to native Swiss citizens, contact rates are lower for all immigrant groups except southern Europeans:

| Origin group | Contact penalty | P-value |
|---|---|---|
| Western & northern Europe | -4.2% | < 0.001 |
| Central & eastern Europe | -6.2% | < 0.001 |
| North & South America | -6.4% | < 0.001 |
| Balkans | -12.6% | < 0.001 |
| Middle East & North Africa | -13.5% | < 0.001 |
| Sub-Saharan Africa | -17.1% | < 0.001 |
| Asia | -18.5% | < 0.001 |
| Southern Europe | not significant | 0.481 |

All regressions are OLS with Lasso-selected controls and search fixed effects, n = 3,251,303.

### Economic significance

Having 4+ years of work experience gives an 11.5% advantage. So for jobseekers from Asia or sub-Saharan Africa, even the highest level of experience is insufficient to offset the ethnic penalty.

### Evidence against statistical discrimination (in plain words)

Several tests suggest the penalties are not driven by rational inference about unobserved productivity:
- Minority groups that are more discriminated against actually have **higher** unobserved productivity signals (age, previous wage)
- Constructing an "unobserved employability index" → ethnic penalties are very similar for low, medium, and high unobserved employability
- More text in the CV description (more information for recruiters) reduces penalties by up to 20% for Asia and sub-Saharan Africa, but not for other groups → information helps a little but doesn't eliminate discrimination

### What this suggests

Results leave large scope for taste-based discrimination (prejudice), but the time-of-day patterns (Block 3) suggest conscious prejudice alone can't explain everything — implicit bias likely plays a role.

---

## Block 3: Time-of-Day Variation (Mechanism)

### What they did (in plain words)

Looked at the same recruiter searching for the same occupation at different times of day. This is within-recruiter, within-occupation variation — only the time changes.

### Results

**Time spent on profiles decreases during the day:**
- 09:00–10:00: 10.5 seconds per profile
- 11:00–11:59: 9.7 seconds (before lunch)
- After lunch: resets to 10.8 seconds
- 17:00–18:00: 9.5 seconds (end of day)

**Ethnic penalties increase as time spent decreases:**
- 09:00–10:00: 11.5% penalty (non-European minorities)
- 11:00–11:59: 13.4% penalty
- After lunch: resets to 11.5%
- 17:00–18:00: 14.7% penalty (P = 0.03 vs. morning)

The pattern is nearly identical for European minorities, but smaller in magnitude.

### What this means

Discrimination is about 20% higher when recruiters are more fatigued and spend less time per profile. The reset after lunch is striking — it mirrors the "depletion of mental resources" literature (Danziger et al. 2011 on judicial decisions). This is consistent with implicit bias theories: discrimination increases when intuitive (rather than deliberate) decision-making takes over.

### What this rules out

- **Not conscious prejudice alone**: conscious prejudice would be constant across the day
- **Not lexicographic search** (immediately screening out minorities without reading CV): recruiters spend almost the same amount of time on minority vs. majority profiles (largest difference < 0.3 seconds)

---

## Block 4: Gender Discrimination

### Results (in plain words)

On average across all occupations: no significant gender penalty (coefficient = -0.00013, P = 0.85, n = 17,369,372).

But this average masks huge heterogeneity across 323 occupations:

| Occupation type | Who is penalized | Penalty size |
|---|---|---|
| Male-dominated (lowest 5 female share) | Women | -6.7% |
| Female-dominated (highest 5 female share) | Men | -12.6% |

The relationship is approximately linear: a 1% increase in the share of women in an occupation is associated with a 0.30% increase in the hiring advantage for women (P < 0.001).

### What this means

Hiring reinforces existing gender segregation. The finding that men are also penalized (in female-dominated occupations) is important — it's hard to explain with standard statistical discrimination theories that assume women are less productive (e.g., because of family responsibilities). This is more consistent with gender stereotype theories.

---

## Counter-arguments & Discussion

| Alternative explanation | Evidence against it |
|---|---|
| Statistical discrimination (rational inference about unobserved skills) | More-discriminated groups have higher unobserved productivity; employability index doesn't change penalties; men also penalized in female jobs |
| Conscious prejudice only | Discrimination varies within-recruiter across the day; resets after lunch |
| Lexicographic search (instant screening) | Time spent on profiles is nearly identical across ethnic groups |
| Unobserved confounders | Validated with anonymized-profile subsample (P = 0.93 for joint ethnic effects) |

### Policy implications

1. Platform data can **continuously monitor** discrimination — cheaper and less ethically fraught than correspondence studies
2. Platforms can be **redesigned** to reduce discrimination: strengthen productivity signals, downplay ethnicity/gender, show side-by-side comparisons
3. Targeted interventions: identify high-discrimination occupations and offer implicit bias training
