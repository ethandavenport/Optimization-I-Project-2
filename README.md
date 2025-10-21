# Optimization I Project 2: Marketing Campaigns

## Links to code notebooks:

| Notebook          | Colab |
|-------------------|-------|
| `linear.ipynb`    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethandavenport/Optimization-I-Project-2/blob/main/linear.ipynb) |
| `mip.ipynb`       | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethandavenport/Optimization-I-Project-2/blob/main/mip.ipynb) |
| `Project_2.ipynb` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethandavenport/Optimization-I-Project-2/blob/main/Project_2.ipynb) |


## In colab, if you make changes to notebooks, use "save in github" at the top of the page to re-commit.
## Download any created csv or other files and re-commit those manually.

| Task                                                     | Description                                                                                                                                                                          | File/Notebook                | Done by | Date | Notes                                                                    |
| -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- | ------- | ---- | ------------------------------------------------------------------------ |
| **1. Linear Program (LP) – Concave ROI Case**            | Formulate and solve the marketing allocation as a **linear program** using Gurobi under the assumption of concave ROI (non-increasing returns).                   |   `linear.ipynb`   |         |      | Maximize total return subject to a $10M budget and platform constraints. |
| **2. Managerial Constraints**                            | Implement the CMO’s constraints: (1) Print+TV ≤ Facebook+Email, (2) Social ≥ 2×(SEO+AdWords), (3) Investment ≤ $3M per platform.                             |    `linear.ipynb`  |         |      | Verify constraint feasibility before solving.                            |
| **4. Mixed Integer Program (MIP) – Nonconcave ROI Case** | Replace the LP with a **mixed integer program** to handle non-monotonic ROI data (`roi_company2.csv`). Introduce binary tier-selection variables for each medium. |    `mip.ipynb`     |         |      | Each tier’s activation controlled by binary variables.                   |
| **5. Cross-Evaluation**                                  | Compare allocations from both firms’ ROI data. Evaluate objective loss when each allocation is applied to the other firm’s ROI estimates.                         |    `mip.ipynb`     |         |      | Quantify robustness and interpret managerial implications.               |
| **6. Minimum Investment Thresholds**                     | Add binary constraints using `min_amount.csv` so each medium is either uninvested or receives ≥ its minimum effective spend.                                   |    `mip.ipynb`     |         |      | Re-solve MIP with these additional thresholds.                           |
| **7. Dynamic Reinvestment Model**                        | Allow 50% reinvestment of monthly returns (e.g., 4% ROI → +0.2M next month). Use `roi_monthly.csv` to compute monthly optimal allocations.                       |    `mip.ipynb`     |         |      | Re-optimize monthly budget given compounding returns.                    |
| **8. Stability Check**                                   | Assess whether monthly allocations are “stable” — i.e., no platform’s budget changes by more than ±$1M month-to-month.                                            |    `mip.ipynb`     |         |      | If unstable, describe how to enforce stability in future MIP.            |
| **9. Visualization and Reporting**                       | Generate clear visuals of ROI tiers, optimal allocation, and comparative returns. Summarize findings in a professionally written report.                        | `Project_2.ipynb`  |         |      | Include graphs, explanation, and embedded code screenshots.              |
| **10. Generalized Code Verification**                    | Ensure no hard-coded numeric values. All computations reference dataframe variables so TA can re-run with new CSVs.                                             |  `Project_2.ipynb` |         |      | Failure to generalize = 10% automatic penalty.                           |
