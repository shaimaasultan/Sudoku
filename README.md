# Sudoku
Scalable Solving for Large Structured CSPs (up to 36×36 and beyond)
# Hybrid Constraint‑Based Sudoku Solver  
### Scalable Solving for Large Structured CSPs (up to 36×36 and beyond)

This repository contains the research, algorithms, and implementation of a hybrid Sudoku solver designed for large \(N \times N\) constraint‑satisfaction problems. The solver integrates propagation, heuristics, and shallow search to achieve near‑polynomial behavior on structured Sudoku‑type grids, significantly outperforming classical backtracking and approaching the efficiency of SAT/CSP solvers on many instances.

---

## 🔍 Overview

The solver combines several complementary techniques:

- **Layer‑based constraint propagation** to eliminate large portions of the search space before branching.
- **MRV (Minimum Remaining Values)** heuristics to guide branching toward the most constrained cells.
- **Shallow backtracking** to avoid exponential blow‑ups typical in naive solvers.
- **Heuristic pruning** to reduce dead‑end exploration.
- **Empirical complexity analysis** using PGFPlots and benchmark datasets.

The system is tested on multiple grid sizes:

- \(9 \times 9\)
- \(12 \times 12\)
- \(16 \times 16\)
- \(25 \times 25\)
- \(36 \times 36\)

---

## 🧠 Key Contributions

- A **layer propagation algorithm** that dramatically reduces candidate sets before search.
- A **hybrid MRV‑guided branching strategy** that minimizes unnecessary exploration.
- A **shallow backtracking engine** tuned for structured CSPs.
- A **scalable implementation** capable of solving very large Sudoku‑type puzzles.
- A full **benchmark suite** with timing curves and complexity analysis.
- A **research paper** (LaTeX) documenting algorithms, theory, and empirical results.

---
## 📂 Repository Structure

---

## 🚀 Running the Solver

### Requirements
- Python 3.9+
- `numpy`
- `matplotlib` (optional, for visualizations)

Install dependencies:

```bash
pip install -r requirements.txt

📬 Contact
Shaimaa Said Soltan  
Mississauga, Ontario, Canada
Email: shaimaasultan@hotmail.com 
GitHub: /shaimaasultan
