# Summary Template for AI Papers

## Naming Convention

Summary files are named: `YYYY-MM-DD-author-et-al-year-summary.md`

Example: `2026-06-03-rafailov-et-al-2023-summary.md`

## Workflow

1. Download PDF to `ai/`
2. Convert: `markitdown paper.pdf -o paper.md`
3. Write summary following the structure below. Use LaTeX for all math: `$...$` for inline, `$$...$$` for display equations
4. **Prefer plain words first, math second.** Always explain the method and training loop in plain words before presenting equations. Math is just a formal expression of the same logic — if the words are clear, the equations follow naturally. A reader should be able to understand the core idea without reading any formulas.
5. **Iterate**: Each paper read is also an opportunity to refine this template.

## Note on AI Papers

AI papers typically follow a "motivation → method → experiments" structure. The method section is the core contribution, often involving a new loss function, architecture, or training procedure derived from mathematical insight. Unlike economics papers (which build identification strategies) or interdisciplinary papers (which synthesize evidence), AI papers are usually about **a new technique** and whether it works.

## Summary Structure

### Overview

- **Paper type**: Method paper, benchmark, survey, analysis, position paper, etc.
- **Core contribution**: The main new idea in one sentence
- **Problem**: What problem does this solve, and why is it hard?
- **Key insight**: The intellectual move that makes the method work
- **Blocks**: List of method/theory blocks + experiment blocks
- **Result summary**: Does it work? How well vs. baselines?

### High-Level Summary

In 3-5 sentences: what is the core insight, why is this a meaningful contribution, and what impact has it had (or might it have)?

### Method Blocks (in paper order)

#### Method Block Template

- **Setup/Problem formulation**: What is the objective being optimized? What is the existing approach?
- **Key equations**: The main formulas, with explanation
- **Derivation**: Step-by-step how the method is derived (high-level + detailed where important)
- **Intuition**: Why this works; what the method is doing mechanistically
- **Theoretical properties**: Any guarantees, equivalences, or analysis

### Experiment Blocks

#### Experiment Block Template

- **Tasks/Datasets**: What benchmarks or tasks are used
- **Baselines**: What is compared against
- **Metrics**: How success is measured
- **Results**: Key numbers, tables, or figures
- **Takeaway**: What does this experiment show about the method?

### Limitations & Future Work

- What the authors flag as limitations
- What questions remain open
