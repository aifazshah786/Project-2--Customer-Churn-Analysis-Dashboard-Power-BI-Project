#  PowerCo Customer Churn Analysis

##  Project Summary

This project analyzes customer churn for PowerCo (SME division).  
The objective was to understand the main drivers of churn and test whether price sensitivity is the primary reason customers leave.

Using exploratory data analysis, feature engineering, and machine learning, we identified the key business drivers behind churn.

---

##  Business Problem

PowerCo is experiencing customer churn in its SME division.

- ~15,000 customers analyzed  
- Nearly 10% churn rate  

Churn directly impacts revenue, margins, and long-term profitability.

The main business hypothesis:

> Is churn primarily driven by customer price sensitivity?

---

## 📊 Exploratory Data Analysis (EDA)

Key observations:

- Annual consumption (`cons_12m`) is one of the strongest churn indicators.
- Time-based features (tenure, months active, contract renewal timing) significantly influence churn.
- Customers close to renewal periods show higher churn probability.
- Consumption behavior differs across churn vs non-churn customers.
- Price variation features exist but are not dominant drivers.

---

##  Feature Engineering

Advanced features created:

- 6-month and 12-month price variation metrics
- Peak vs off-peak pricing differences
- Consumption trend indicators
- Margin-based variables
- Contract lifecycle features

Correlation analysis showed multicollinearity among some engineered price features, requiring feature reduction before modeling.

---

##  Model Insights (Feature Importance)

Top drivers of churn:

1. Annual Consumption (`cons_12m`)
2. Net Margin
3. Gross Margin (Electricity)
4. Meter Rent Forecast
5. Time-based Features (tenure, months_active)

Price sensitivity variables were present but not among the strongest predictors.

---

#  Executive Summary (Final Conclusion)

### 🔎 Churn Overview

- Churn is high in the SME division  
- Nearly 10% churn across ~15k customers  

The likelihood of churn can be measured and predicted using customer consumption, margin, and lifecycle data.

A sensitivity analysis was conducted to evaluate the impact of price changes on churn behavior.

---

###  Key Findings

- Price sensitivity is **not** the primary driver of churn.
- Net and gross margins on electricity are the largest contributors to churn over the past 12 months.
- Customer consumption behavior is a stronger indicator than price variation.
- Contract lifecycle timing plays a major role.

---

##  Final Takeaway

Churn at PowerCo is driven more by structural and behavioral factors than by price sensitivity.

To effectively reduce churn, the company should prioritize:

- Contract renewal management
- High-consumption customer monitoring
- Margin-based segmentation
- Customer engagement strategies

Instead of relying heavily on discounts, PowerCo should adopt a data-driven retention strategy.

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
