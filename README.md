# Customer Churn & Retention Analysis

A SQL-first analysis of customer churn using [DuckDB](https://duckdb.org/) inside a Jupyter notebook, with
Matplotlib and Seaborn for visualization. The dataset covers 64,374 subscription customers, with features
including tenure, usage frequency, support calls, payment delay, subscription tier, contract length, and total spend.

## Questions explored

1. What is the overall churn rate?
2. How does churn vary by subscription tier (Basic / Standard / Premium) and contract length (Monthly / Quarterly / Annual)?
3. When in the customer lifecycle is churn most likely (tenure buckets)?
4. How do support call volume and payment delays relate to churn?
5. Which customer segments are highest risk (subscription × contract heatmap, multi-signal risk profile, age groups)?
6. How do churned and retained customers differ on key behavioral metrics?

The notebook ends with a findings-and-recommendations table that turns each pattern into a retention action
(e.g., incentives for longer contracts, onboarding check-ins for new customers, proactive outreach after repeated support calls).

## Run it

1. Install dependencies: `pip install duckdb pandas matplotlib seaborn`
2. Place `customer_churn_dataset-testing-master.csv` in the same folder as the notebook (or update `CSV_PATH` in the loading cell).
3. Run `customer_churn_analysis.ipynb` from top to bottom.
