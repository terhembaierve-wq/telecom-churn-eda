# Telecom Customer Churn: Exploratory Data Analysis

Group project (my role: **Data Exploration Lead**). Exploratory analysis of 7,043 telecom customers to understand why customers leave and which segments are most at risk.

## Key findings
- **Dataset:** 7,043 customers, 21 variables. Overall churn rate is **26.5%** (1,869 customers).
- **Data quality:** no duplicates or null values. 11 invalid `TotalCharges` values were found, all belonging to zero-tenure customers, and were corrected.
- **Strongest churn drivers:**
  - Month-to-month contracts: 42.7% churn vs 2.8% on two-year contracts
  - Fiber optic internet: 41.9%
  - Electronic check payments: 45.3%
  - No online security or tech support: about 42% vs about 15% with them
  - Short tenure: median 10 months for churned customers vs 38 for retained
- **Weak drivers:** gender and phone service.
- **Modelling note:** `TotalCharges` is strongly correlated with `tenure` (r = 0.83), so it adds little independent signal.

## What the notebook covers
- Data inspection and data dictionary
- Data-quality checks and cleaning
- Churn distribution and class imbalance
- Churn rate by categorical feature (ranked by spread)
- Numeric features vs churn (distributions, correlation heatmap)
- Contract type x tenure band analysis
- Multicollinearity check

## Tools
Python (pandas, NumPy, matplotlib, seaborn), Google Colab, Jupyter, VS Code

## Files
- `02_Group_2_Exploratory_Data_Analysis.ipynb`: the full analysis

## Data source
[https://www.mavenanalytics.io%2Fblog%2Fmaven-churn-challenge]

## Author
Terhemba (Jason) Ierve: [LinkedIn](https://www.linkedin.com/in/terhemba-ierve-371a15171)
