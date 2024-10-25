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

- **Loan Approval and Risk**: The analysis highlights key factors, such as income-to-loan ratio and age, that significantly influence loan approval and risk levels.
- **Demographic Insights**: Certain age groups and income levels correlate with higher or lower loan approval rates, providing a better understanding of target customer demographics.
- **High-Risk Identification**: Effective identification of high-risk customers enables targeted risk mitigation and tailored marketing efforts.

### Summary for Stakeholders

**Loan Approval Strategies**  
The analysis reveals distinct patterns in loan approval likelihood based on income and demographic segments. By focusing on customers with favorable income-to-loan ratios, the bank can strategically adjust its loan approval criteria to maximize successful repayments.

**Targeted Marketing and Customer Segmentation**  
The insights into customer demographics enable the bank to identify and prioritize marketing efforts toward low-risk customer segments, such as those within specific income brackets or family sizes. Marketing initiatives can be tailored to address the unique needs and financial behaviors of these groups.

**Risk Management Enhancement**  
With the identification of high-risk customer characteristics, the bank can implement more robust risk assessment protocols. Tailoring loan products or setting stricter approval criteria for higher-risk segments helps manage potential defaults more effectively.

**Improving Loan Products Based on Demographic Trends**  
The demographic insights suggest that certain customer groups may respond positively to custom loan products or financial advice that aligns with their unique income and loan needs. Focusing on these groups can improve customer satisfaction and long-term retention.

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
