---
marp: true
theme: default
paginate: true
header: "Customer Spending Analysis"
footer: "Newton School of Technology - Data Visualization & Analytics | Capstone 2"
---

# Customer Spending Analysis
## Data Visualization & Analytics Capstone 2

**Sector:** Finance
**Team ID:** C-6
**Team Members:** Veer Shah, Meet Ramatri, Ronak Satya Swarup Das
**Institute:** Newton School of Technology

---

# Context & Problem Statement

- **Sector Context:** Financial institutions face the challenge of accurately assessing creditworthiness while understanding modern consumer behavior.
- **Stakeholder:** Senior Risk Management and Strategy Teams
- **Core Business Question:** How do customer spending patterns and transaction velocity impact their probability of loan default?
- **Objective:** Analyze spending patterns to predict potential default risks and provide actionable insights for optimized lending strategies to mitigate credit risk.

---

# Data Engineering

- **Source:** Synthetic Finance Dataset (TestDataBox)
- **Size and Coverage:** 50,000+ rows across 8 distinct tables (customers, accounts, loans, transactions, branches, etc.).
- **Major Cleaning Steps:** 
  - Handled 2% missing values (nulls) and 1% duplicate records.
  - Resolved inconsistent formatting, mixed date formats, and corrected 1% intentional text anomalies.
  - Standardized customer demographics and account types.
- **Data Dictionary Summary:** Key attributes include transaction frequency, loan-to-balance ratios, account statuses, and withdrawal behaviors.

---

# KPI Framework

- **Transaction Frequency (Velocity):** Tracks the volume of transactions over a period. High velocity combined with low balances indicates cash instability.
- **Withdrawal-to-Deposit Ratio:** Tracks cash outflow vs. inflow. Crucial for detecting early signs of liquidity issues.
- **Loan-to-Balance Ratio:** Total loan principal compared to historical cash reserves. Identifies over-leveraged accounts.
- **Default Probability (Risk Score):** A derived metric using demographic data and spending behavior to estimate the likelihood of entering the 'Overdue' phase.

---

# Key EDA Insights

1. Customers entering the 'Overdue' phase exhibit vastly different Loan-to-Balance ratios compared to those with current loans.
2. Defaulters show a distinct and statistically significant divergence in their withdrawal vs. deposit behavior prior to default.
3. A customer's banking velocity and debt ratio are powerful indicators of future financial stability.
4. Transaction frequency heavily correlates with the overall risk profile of the account.
5. Specific age brackets and customer types demonstrate inherently higher baseline default rates.

---

# Advanced Analysis

- **Statistical Method 1:** T-Test applied to confirm that transaction frequency directly and significantly affects default risk.
- **Statistical Method 2:** Chi-Square test utilized to prove that customer demographics (Age, Customer Type) significantly influence default probabilities.
- **Root Cause Finding:** Aggregation via 6 specialized pivot tables isolated the exact demographics and account types failing to meet creditworthiness standards.

---

# Dashboard Overview

- **Objective:** Convert complex statistical proof into 6 easily digestible visuals for stakeholders.
- **Executive View:** High-level summary of portfolio health, tracking overall default rates and high-risk demographic exposure.
- **Operational View:** Granular analysis of individual transaction velocities, loan-to-balance ratios, and early warning triggers.
- **Filters and Drilldowns:** Interactive segmentation by Customer Type, Account Type, Age Bracket, and Branch Location.

---

# Top Insights

1. **Loan-to-Balance Ratios:** Overdue accounts had significantly disproportionate loan principals relative to their historical cash reserves.
2. **Demographic Influence:** Age and Customer Type are not just descriptive but highly predictive factors in determining default likelihood.
3. **Behavioral Precursors:** A widening 'Withdrawal-to-Deposit' ratio is a reliable early warning signal of impending loan default.

---

# Recommendations

1. **Loan-to-Balance Restrictions:** Implement a hard cap on lending principal based on historical cash reserves to mitigate over-leveraging.
2. **Targeted Demographics:** Direct marketing and premium loan product offerings toward the lowest-risk age brackets to optimize portfolio profitability.
3. **Transaction Velocity Triggers:** Monitor real-time 'Withdrawal-to-Deposit' ratios as an early warning system to flag high-risk behavior before a formal default occurs.

---

# Impact

- **Expected Outcome:** 
  - Reduced financial loss from loan defaults by restricting principal for risky accounts.
  - Increased loan portfolio profitability through targeted low-risk lending.
  - Proactive intervention capabilities via real-time monitoring.
- **Priority:** High
- **Feasibility:** High (Utilizing existing transaction and balance data infrastructure)

---

# Limitations

- **Data Constraints:** The dataset used is synthetic (~7% intentionally introduced noise), requiring careful anomaly filtering to avoid skewed insights.
- **Method Constraints:** Statistical tests assume independent variables, but financial behaviors are often interconnected.
- **Scope Limitations:** Analysis is confined to available demographic and internal transaction data, lacking external economic indicators (e.g., inflation, employment rates).

---

# Next Steps

- **Future Extensions:** 
  - Integrate external macroeconomic data to improve default prediction accuracy.
  - Deploy a machine learning model (e.g., Random Forest or XGBoost) to automate risk scoring in real-time.
- **Closing Summary:** By leveraging transaction velocity and loan-to-balance ratios, the bank can shift from reactive default management to proactive risk mitigation, ensuring a healthier loan portfolio and sustained profitability.
