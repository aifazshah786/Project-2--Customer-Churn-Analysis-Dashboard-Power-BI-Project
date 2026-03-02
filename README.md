#  PowerCo Customer Churn Analysis

##  Project Summary

This project analyzes customer churn for PowerCo (an energy company).  
The goal is to understand why customers leave and test whether churn is mainly driven by price sensitivity.

We used data analysis, feature engineering, and machine learning to identify the key drivers of churn and provide business recommendations.

---

##  Business Problem

PowerCo is facing customer churn which impacts:

- Revenue
- Profitability
- Customer lifetime value

The main hypothesis from the business was:

> Is churn driven by customers' price sensitivity?

This project tests that hypothesis using data.

---

## 📊 Exploratory Data Analysis (EDA)

Key findings from visual analysis:

- Annual consumption (`cons_12m`) is one of the strongest indicators of churn.
- Time-related features (tenure, months active, contract renewal timing) strongly influence churn.
- Customers close to contract renewal are more likely to churn.
- High consumption customers behave differently compared to low consumption customers.
- Price variation features exist but are not the dominant factor.

---

## Feature Engineering

We created advanced features such as:

- 6-month and 12-month price variation
- Peak vs off-peak price differences
- Consumption trends
- Margin-based metrics
- Contract lifecycle indicators

Correlation analysis showed high multicollinearity among some engineered price variables, which required feature selection.

---

## Model Insights (Feature Importance)

Top drivers of churn:

1. Annual Consumption (`cons_12m`)
2. Net Margin
3. Meter Rent Forecast
4. Power Margin Variables
5. Time-based Features (tenure, months_active)

Price sensitivity features were present but not among the strongest predictors.

---

## ❓ Hypothesis Result

Is churn mainly driven by price sensitivity?

**No.**

Price sensitivity is a weak contributor, but the main drivers are:

- Customer consumption behavior
- Profitability structure (margins)
- Contract lifecycle timing
- Fixed recurring charges

Churn is more behavioral and structural rather than purely price-driven.

---

##  Business Recommendations

Based on the analysis:

- Focus on contract renewal retention strategies.
- Monitor high-consumption customers to prevent bill shock.
- Segment customers by profitability.
- Improve onboarding for new customers.
- Launch targeted retention campaigns before contract expiry.

---

## 📂 Project Workflow

- Task 1 – Business Understanding
- Task 2 – Exploratory Data Analysis
- Task 3 – Feature Engineering
- Task 4 – Modeling & Feature Importance Analysis

---

## 🏁 Final Conclusion

Customer churn at PowerCo is influenced more by usage behavior and contract timing than price sensitivity.
To reduce churn, the company should focus on lifecycle management and customer behavior tracking instead of only adjusting pricing.

---

##  Tools Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

---
