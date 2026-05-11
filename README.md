# Telco Customer Churn Analysis

**Future Interns — Task 2 | Data Analysis Internship**

## Project Overview

Analysis of a telecommunications company's customer dataset containing **7,043 customers** to identify key drivers of churn, high‑risk customer segments, and revenue impact. The findings are presented in a **4‑page interactive Power BI dashboard** with actionable recommendations to reduce customer attrition.

## Tools Used

- **Python (Jupyter Notebook)**
- **Pandas / NumPy**
- **Matplotlib / Seaborn**
- **Power BI Desktop**

## Dataset

- Raw dataset: **7,043 records, 21 columns**
- Cleaned dataset: **7,043 records, 24 columns**
- Overall churn rate: **26.5%**

## What I Did

- Loaded and inspected the raw data
- Cleaned `TotalCharges` (converted to numeric, filled 11 missing values with `MonthlyCharges`)
- Engineered new features: `Churn_Flag`, `Tenure_Group`, `Charge_Group`
- Performed exploratory data analysis in Python (churn by contract, tenure, charges, services, demographics)
- Built a **4‑page Power BI dashboard**

## Dashboard Pages

- **Page 1 — Churn Overview**  
  KPIs: Total customers (7,043), churned (1,869), retained (5,174), overall churn rate (26.54%). Churn by contract type, payment method, and internet service.

- **Page 2 — Tenure and Lifetime Analysis**  
  Tenure distribution (churned vs retained), churn rate by tenure group, average tenure comparison (churned: 18 months vs retained: 37.6 months), average monthly charges comparison.

- **Page 3 — Customer Segment Analysis**  
  Churn by gender, senior citizen status, partner status, dependents. Service impact: paperless billing, tech support, online security.

- **Page 4 — Retention Insights and Recommendations**  
  High‑risk customer count (~2,128), monthly revenue lost (~$100K). Top risk factor combinations (e.g., month‑to‑month + fiber optic + electronic check). Actionable recommendations to reduce churn.

## Key Insights

- **Overall churn rate:** 26.5% (1,869 of 7,043 customers)
- **Contract type** – Month‑to‑month customers have churn rate **~45%** (vs. ~20% for one‑year, ~3% for two‑year)
- **Internet service** – Fiber optic customers churn at **~42%** (DSL ~19%, no internet ~7.4%)
- **Payment method** – Electronic check customers churn at **~45%** (other methods ~15‑20%)
- **Tenure** – Churned customers average only **18 months** (retained: 37.6 months)
- **Monthly charges** – Churned customers pay **$74.44** vs retained **$61.27**
- **Senior citizens** churn at **41.7%** (vs 23.6% for non‑seniors)
- Customers **without online security or tech support** have churn rates above 40%
- **Monthly revenue lost** from churn estimated at **~$100,000**

## Recommendations

1. Convert month‑to‑month customers to long‑term contracts with incentives
2. Improve fiber optic service quality and customer support
3. Incentivize electronic check payers to switch to automatic payments
4. Focus retention efforts on first 12 months (onboarding, loyalty perks)
5. Bundle online security and tech support with internet plans
6. Provide tailored support for senior citizen segment

## Files in This Repository

- `ChurnAnalysis.ipynb` — Python cleaning, feature engineering, and EDA notebook
- `cleaned_churn_data.csv` — Exported clean dataset for Power BI 
- `Telco_Churn_Dashboard.pbix` — Power BI dashboard file
- `screenshots/` — Dashboard page screenshots
