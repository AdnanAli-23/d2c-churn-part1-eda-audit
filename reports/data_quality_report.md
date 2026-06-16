# Data Quality Report

## Dataset Overview

The analytical dataset was created by combining customer, order, web activity, support ticket, intervention, and churn datasets.

### Final Dataset

- Total Customers: 2,400
- Total Features: 23
- Target Variable: `churn_next_60d`

---

## Data Completeness

### Missing Values

All datasets were inspected for missing values.

**Findings**

- No significant missing values were identified in key analytical fields.
- The merged analytical dataset was suitable for exploratory analysis and hypothesis testing.

**Impact**

No imputation was required.

---

## Duplicate Records

### Customer Dataset

- Customer IDs were unique.
- No duplicate customer records were detected.

### Order Dataset

- Order IDs were unique.
- No duplicate transactions were found.

### Support Dataset

- Ticket IDs were unique.

**Impact**

Duplicate records were not expected to influence analysis results.

---

## Join Validation

The following joins were performed:

1. Customer + Churn
2. Customer + Web Activity
3. Customer + Intervention History

### Validation Results

- Customer counts remained consistent after joins.
- No unexpected row loss occurred.
- Customer IDs matched correctly across datasets.

---

## Data Consistency Checks

### Snapshot Date

All customer records shared the same snapshot date.

### Customer Identifier

Customer IDs were consistently formatted and unique.

### Categorical Variables

The following variables contained valid category values:

- Age Group
- Loyalty Tier
- Acquisition Channel
- Marketing Consent
- Preferred Category
- City Tier

No invalid category labels were detected.

---

## Outlier Review

Continuous variables reviewed:

- Sessions
- Product Views
- Campaign Clicks
- Last Visit Days Ago
- Campaign Cost
- Order Amount

Observed outliers appeared to represent genuine customer behavior and were retained.

---

## Potential Data Leakage Review

The target variable was:

- `churn_next_60d`

Variables that could directly reveal future churn were not included in feature creation.

No obvious leakage issues were identified during exploratory analysis.

---

## Data Quality Assessment

### Strengths

- Clean customer identifiers
- Consistent joins
- No significant missing values
- No duplicate records
- Well-defined churn target

### Limitations

- Analysis is based on a single snapshot period.
- Certain demographic variables showed weak predictive power.
- Some behavioral relationships require validation through predictive modeling.

---

## Final Conclusion

The dataset demonstrates good overall quality and is suitable for customer churn analysis, exploratory data analysis, customer segmentation, and predictive modeling.