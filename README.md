# **Banking Loan Analytics - SQL Data Analysis**

## Project Overview

This project explores customer loan behaviors and demographic trends to understand risks, customer segmentation, and potential predictors of loan defaults. The dataset provides detailed information on demographics and financial data, such as income, age, family size, and loan amounts. The analysis performs data wrangling, feature engineering, and core SQL queries to uncover insights for decision-making.

## Table of Contents

- [Introduction](#introduction)
- [Step 1: Imports](#step-1-imports)
- [Step 2: Data Exploration, Cleaning, and Preparation](#step-2-data-exploration-cleaning-and-preparation)
- [Step 3: Analytical Queries](#step-3-analytical-queries)
- [Step 4: Results and Evaluation](#step-4-results-and-evaluation)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)
- [References](#references)

## Introduction

This SQL analysis evaluates customer loan data to identify significant factors influencing loan risk and customer demographics. By analyzing loan and customer information, this project provides insights into customer behavior and key predictors of loan outcomes, which can inform decisions in customer targeting and risk assessment.

---

## Step 1: Imports

**Database Setup and Imports**  
To get started, set up a SQL-compatible database (MySQL, PostgreSQL, etc.) and load the datasets provided in `Bank_Personal_Loan_Modelling` and `Submission_Approval_Datetime.csv` tables.

---

## Step 2: Data Exploration, Cleaning, and Preparation

### Exploring the Data

The dataset includes the following key features:
- **Age**
- **Experience**
- **Income**
- **Family Size**
- **Loan Amount**
  
These attributes help uncover insights into customer loan behaviors and enable segmentation by demographics and loan characteristics.

### Checking for Missing Values

An initial query confirms that no missing values are found in essential demographic variables, ensuring data integrity.

### Duplicate Removal

An initial check identified duplicate entries in customer IDs, which were removed to avoid analysis bias. The cleaned dataset is now ready for analysis.

### Outlier Detection

Outliers in the data (e.g., unusually high income or loan amounts) were examined and treated to avoid skewing the analysis results.

---

## Step 3: Analytical Queries

1. **Customer Segmentation**: The dataset is segmented by customer demographics, such as income and family size, to understand target groups.
2. **Loan Approval and Risk**: Queries analyze loan approval rates and high-risk loans based on demographics.
3. **Income-to-Loan Ratio**: A calculated ratio helps assess customer affordability and loan risk.
4. **Default Prediction**: Potential predictors of default risk are identified based on customer characteristics.

---

## Step 4: Results and Evaluation

### Key Performance Indicators (KPIs)

- **Loan Approval Rate**: Percentage of approved loans provides insight into general acceptance trends.
- **Default Rate**: Percentage of defaulted loans gauges risk levels.
- **Income-to-Loan Ratio**: Assesses customer affordability.
- **High-Risk Customer Percentage**: Percentage of high-risk customers based on demographic indicators.

### Analytical Findings

1. **Customer Segmentation**: Key segments of customers by age, income, and family size.
2. **High-Risk Indicators**: Income and age patterns correlate with default risks.
3. **Data Quality**: The dataset is validated with no missing values or duplicates, ensuring accuracy.

---

## Conclusion

### Key Insights

- **Customer Segmentation**: Key segments of customers by age, income, and family size.

   
- **Loan Approval and Risk**: Only 9.6% of applicants currently hold personal loans, with an average income of $144.75K among those approved, compared to $66.24K for non-approved applicants.
  
- **Demographic Insights**: The average age of approved applicants is 45.07 years, and those with higher credit card usage (average 3.91) are more likely to be approved, suggesting that age, income, and credit card usage patterns play significant roles in loan approval.
   
- **High-Risk Identification**: Applicants with lower credit card usage (average 1.73 among non-approved applicants) are at a higher risk of default, pointing to credit card usage as a valuable predictor for risk assessment.

- **Operational Efficiency**: With an average turnaround time of 95.75 hours and a maximum of 168 hours for loan approvals, there are clear opportunities to optimize loan processing times.
   
### Summary for Stakeholders

**Loan Approval Strategies**  
The analysis shows that 9.6% of applicants receive personal loans, indicating a niche market segment that can be targeted more effectively. Those approved have an average income of $144.75K, compared to $66.24K for those not approved, suggesting that income is a critical factor for loan eligibility. Additionally, with an average turnaround time of 95.75 hours for loan approvals, we have insights that may help to refine and expedite the approval process.

**Targeted Marketing and Customer Segmentation**  
We identified that 90.4% of applicants do not hold personal loans, signaling a large untapped market. By targeting applicants with an income-to-loan ratio above a certain threshold, the bank can focus on customers who are more likely to qualify for loans. For example, higher-income groups not only have greater loan approval odds but also tend to have higher credit card usage (averaging 3.91 for those approved), which may signify reliable repayment habits.

**Risk Management Enhancement**  
The data suggests that high-income applicants with average credit card usage rates of 3.91 are less likely to default, compared to those with lower usage rates (average of 1.73). Identifying and focusing on applicants fitting this profile, especially within the 23 to 67 age range, may help mitigate risks and tailor loan products more precisely.

**Improving Loan Products Based on Demographic Trends**  
Demographic analysis showed that loan applicants approved for loans tend to average 45.07 years in age and $144.75K in income. Additionally, 168 hours was noted as the longest approval turnaround time, providing a benchmark to improve and expedite the approval process. With this insight, the bank can focus on crafting loan products or outreach specifically for higher-income, mid-age customers who meet these characteristics.

---

## How to Run

1. **Database Setup**: Import the `Bank_Personal_Loan_Modelling` and `Submission_Approval_Datetime.csv` datasets into your SQL environment.
2. **Run Queries**: Execute the queries in `Banking-Loan-Analytics-Script.sql` to perform the analysis.
3. **Analyze Results**: Use the KPIs and insights to interpret loan and customer patterns.

---

## References

- [SQL Documentation](https://www.mysql.com/)
- [Bank Personal Loan Modelling Data](https://www.kaggle.com/code/pritech/bank-personal-loan-modelling)

---
