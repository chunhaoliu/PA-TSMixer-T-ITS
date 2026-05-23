# CLAUDE.md — T-ITS Manuscript

## Paper Status
- Target: IEEE Transactions on Intelligent Transportation Systems
- 9 pages, 41 references, 7 tables, 3 figures
- Complete and compilable: `pdflatex T-ITS_Manuscript.tex`

## Core Rules

### 1. Think Before Editing
- The `.tex` file is the single source of truth. PDF is generated, never hand-edited.
- Before changing a result number, verify it matches the JSON in `results/final/final_comparison_v2.json`.
- When adding a reference, verify it's a real paper from a top venue (IEEE Trans, ICLR, NeurIPS, ICML, AAAI, CVPR, Nature).

### 2. Simplicity First
- No new sections without checking page budget (9 pages, tight).
- No new tables that duplicate information already in the text.
- Every figure must have a specific conclusion it supports — no "decorative" figures.

### 3. Surgical Changes
- Reference list is in order of appearance. When adding a reference in the middle, renumber all subsequent citations.
- Tables use `\toprule`, `\midrule`, `\bottomrule` (booktabs). No vertical rules.
- Figure labels: `fig:arch`, `fig:analysis`, `fig:trajectory`, etc. Consistent prefix.

### 4. Goal-Driven Execution
- Compile check: `pdflatex T-ITS_Manuscript.tex` must produce zero errors and zero warnings.
- Cross-reference check: all `\ref{...}` and `\cite{...}` must resolve.
- Page count: 8-10 pages (T-ITS limit). Currently 9.

## Build
```bash
cd "D:/OneDrive/02_Study/2024_NJUST/Trajectory  Prediction/ATP__Project/T-ITS_Manuscript"
pdflatex T-ITS_Manuscript.tex
pdflatex T-ITIS_Manuscript.tex  # second pass for references
```
