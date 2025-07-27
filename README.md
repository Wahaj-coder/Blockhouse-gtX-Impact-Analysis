# Blockhouse-gtX-Impact-Analysis
This repository contains my solution for modeling the temporary impact function **gt(X)** and designing an execution allocation strategy to minimize slippage, as part of the Blockhouse work trial task.
The project involves:
- Modeling **gt(X)** based on Level 1 order book data.
- Comparing linear (βₜ) approximations with actual computed slippage.
- Developing an allocation strategy to buy **S = 60,000 shares** across **N = 390 minutes** while minimizing total impact.
- Analyzing 3 ticker datasets: FROG, SOUN, and [Third Ticker].

---

## Repository Structure
/
├── FROG_gtX_Impact_Analysis.ipynb # Complete analysis for FROG ticker
├── SOUN_gtX_Impact_Analysis.ipynb # Complete analysis for SOUN ticker
├── [TICKER]_gtX_Impact_Analysis.ipynb # Complete analysis for 3rd ticker
├── gtX_Modeling_Explanation.pdf # Detailed write-up for Task 1 & Task 2
└── README.md # This file

---

## Instructions to Run
1. Download any of the `.ipynb` files.
2. Open in **Jupyter Notebook** or **Google Colab**.
3. Run cells sequentially.
4. Ensure you have placed the respective ticker CSV files in correct folder paths as defined in the code.

---

## Notes
- All computations are performed using **Level 1 order book data**.
- Allocation strategy is dynamically computed based on **inverse gt(X)**.
- Regression models are used to benchmark βₜ predictions but the final allocation strategy is slippage-based.
