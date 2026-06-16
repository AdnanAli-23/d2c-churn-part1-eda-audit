# Customer Churn Analysis - Part 1 (Data Audit, EDA & Business Understanding)

## Project Objective

The objective of this project is to perform a complete data audit and exploratory data analysis (EDA) to understand customer churn behavior and identify key business risks before predictive modeling.

---

## Repository Structure

```text
part1-eda-audit/

├── notebooks/
│   └── eda_audit.ipynb
│
├── reports/
│   ├── data_quality_report.md
│   └── business_memo.md
│
├── README.md
├── requirements.txt
```

---

## Datasets Used

- Customers
- Orders
- Support Tickets
- Web Activity
- Churn Labels
- Intervention History

---

## Data Audit Activities

The following checks were performed:

- Missing value analysis
- Duplicate record detection
- Join validation
- Data consistency checks
- Target variable validation
- Potential leakage review
- Outlier review

---

## Exploratory Data Analysis

EDA covered:

- Customer demographics
- Loyalty tiers
- Acquisition channels
- Website engagement
- Customer inactivity
- Order behavior
- Spending behavior
- Return behavior
- Support ticket behavior
- Campaign history
- Churn distribution

---

## Churn Hypotheses Evaluated

1. Churn is a significant business problem
2. Younger customers churn more frequently
3. Loyalty tier impacts churn
4. Customer inactivity increases churn
5. Lower website engagement increases churn
6. Abandoned cart activity impacts churn
7. Acquisition channel impacts churn
8. Marketing consent affects churn
9. Returned orders increase churn
10. Reopened support tickets increase churn
11. High spending customers churn less frequently
12. Customers with more orders churn less frequently

---

## Key Findings

- Customer inactivity is the strongest churn signal.
- Website engagement is strongly associated with retention.
- Higher order frequency reduces churn.
- Higher spending customers are more loyal.
- Loyalty programs improve retention outcomes.
- Organic and referral customers show lower churn.

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Outcome

The analysis identified several business-driven churn patterns and produced actionable recommendations for customer retention and future predictive modeling.