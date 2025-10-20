# Optimization I Project 2: Marketing Campaigns

## Links to code notebooks:

| Notebook          | Colab |
|-------------------|-------|
| `linear.ipynb`    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethandavenport/Optimization-I-Project-2/blob/main/linear.ipynb) |
| `mip.ipynb`       | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethandavenport/Optimization-I-Project-2/blob/main/mip.ipynb) |
| `Project_2.ipynb` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ethandavenport/Optimization-I-Project-2/blob/main/Project_2.ipynb) |


## In colab, if you make changes to notebooks, use "save in github" at the top of the page to re-commit.
## Download any created csv or other files and re-commit those manually.


| Task                               | Description                                                                                                                                                | File/Notebook   |  Done by  |  Date  | Notes |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------|-----------|--------| ------|
| **2. Optimal 2019 Portfolio**      | Find the portfolio that minimizes the daily average CVaR using the 2019 data. Use β = 0.95 and R = 0.02%.                                                  |          .ipynb |           |        |       |
| **2a. 2020 CVaR**                  | Recompute the 95%-CVaR for 2020 by evaluating the CVaR objective using the 2019-optimized x and 2020 returns.                                              |          .ipynb |           |        |       |
| **2b. NDX CVaR**                   | Calculate the 95%-CVaR of the NDX index for the same periods (2019 in-sample and 2020 out-of-sample) for comparison.                                       |          .ipynb |           |        |       |
| **3. Different Beta Values**       | Re-run the 2019 CVaR minimization with β = 0.90 and β = 0.99 and describe how changing β shifts the portfolio allocations.                                 |          .ipynb |           |        |       |
| **4. Conservative Risk Mgmt**      | Replace the objective with minimizing the maximum monthly β-CVaR (the worst single-month tail loss) using 2019 data and compare with the Part 2 portfolio. |          .ipynb |           |        |       |
| **5. Monthly Updates**             | Implement a rolling monthly re-optimization for 2020 (each month’s portfolio chosen using the previous 12 months of daily returns).                        |          .ipynb |           |        |       |
| **6. Stable Portfolio**            | Check whether consecutive monthly portfolio weights change by no more than ±0.05 per instrument (i.e., stable).                                            |          .ipynb |           |        |       |
| **7. PDF Report Format**           | Produce a professionally formatted PDF report containing narrative, figures, and executable code chunks.                                                   |          .ipynb |           |        |       |
| **8. CSV + Generalizability**      | Include a top-level `pd.read_csv(...)` call (clearly commented) and ensure all code is generalized (no hard-coded values).                                 |          .ipynb |           |        |       |
