# Summary Template for Economics Papers

## Naming Convention

Summary files are named: `YYYY-MM-DD-author-et-al-year-summary.md`

Example: `2026-06-01-bohren-et-al-2019-summary.md`

## Workflow

1. Download PDF to `economics/`
2. Convert: `markitdown paper.pdf -o paper.md`
3. Write summary following the structure below. Use LaTeX for all math: `$...$` for inline, `$$...$$` for display equations (renders on both GitHub and Obsidian)
4. **Iterate**: Each paper read is also an opportunity to refine this template. If the current structure doesn't capture something important, or a section feels redundant, update this template based on that experience.

## Summary Structure

### Overview

- **Number of blocks**: How many theory models + experiments/empirical analyses
- **Block purposes**: What each block does in the paper
- **Block relationships**: How blocks connect and build on each other
- **Research question(s)**: The main question(s) the paper addresses
- **Conclusion**: Final answer/takeaway

### Blocks (in paper order)

#### Theory Block Template

- **Assumptions**: What the model assumes
- **Key formulas**: The main equations used in derivation
- **Conclusion/Result**: The proposition or main result
- **Derivation (high-level)**: How the proof/derivation works at a high level
- **Intuition**: Why this result makes sense intuitively; why the derivation should hold

#### Experiment Block Template

- **Participants**: How many, recruited from where, payment (bonus rules)
- **Design/Game**: What exactly participants do
- **What it captures (high-level)**: What variation this design exploits
- **Results**: Specific regressions run, interpretation of coefficients, and findings

#### Observational/Empirical Block Template

- **Data**: What dataset, source, time period, sample size
- **Method**: Specific regressions/statistical procedures and their interpretation
- **Results**: Findings and how they relate to the theory
