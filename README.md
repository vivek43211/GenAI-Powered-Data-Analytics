# GenAI-Powered-Data-Analytics
This is GenAI Powered Data Analytics 
# Task -1  Tata GenAI Data Analytics – Delinquency Risk EDA Project

![EDA](https://img.shields.io/badge/Task-Exploratory%20Data%20Analysis-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Domain](https://img.shields.io/badge/Domain-Credit%20Risk-orange)
![Tools](https://img.shields.io/badge/Tools-GenAI%20%7C%20EDA%20%7C%20Excel-blueviolet)

---

## 📌 Project Overview

This project is part of the **Tata GenAI Powered Data Analytics Virtual Job Simulation**.

The objective was to perform **Exploratory Data Analysis (EDA)** on a customer credit dataset to:
- Understand customer financial behavior  
- Identify delinquency risk patterns  
- Improve dataset quality for predictive modeling  

---

## 🎯 Problem Statement

Financial institutions need to identify **customers likely to default** in order to reduce financial risk.

### 🔍 Objectives:
- Analyze customer credit behavior  
- Detect missing and inconsistent data  
- Identify key predictors of delinquency  
- Generate actionable insights  

---

## 📂 Dataset Overview

| Attribute | Details |
|----------|--------|
| 📊 Total Records | 500 |
| 📈 Total Features | 19 |
| 🎯 Target Variable | Delinquent_Account |
| 🔢 Numerical Features | Income, Loan_Balance, Credit_Score, DTI, Utilization |
| 🔤 Categorical Features | Employment_Status, Payment History, Card Type |

---

## ⚙️ Step-by-Step Procedure

### 1️⃣ Data Understanding
- Loaded dataset and reviewed structure  
- Identified numerical and categorical variables  
- Checked for duplicates and anomalies  

---

### 2️⃣ Data Cleaning & Preprocessing

#### 🔍 Missing Value Analysis

| Column | Missing % | Method | Reason |
|--------|----------|--------|--------|
| Income | 7.8% | Median Imputation | Handles skewed data |
| Loan_Balance | 5.8% | Predictive Imputation | Uses related features |
| Credit_Score | 0.4% | Mean Imputation | Minimal impact |

---

#### ⚠️ Data Issues Fixed
- Standardized inconsistent values in `Employment_Status`
- Removed `Customer_ID` (non-predictive feature)
- Cleaned categorical inconsistencies

---

### 3️⃣ Exploratory Data Analysis (EDA)

#### 📊 Univariate Analysis
- Distribution of:
  - Age  
  - Income  
  - Credit Score  

#### 📈 Bivariate Analysis
- Credit Utilization vs Delinquency  
- Debt-to-Income Ratio vs Delinquency  
- Loan Balance vs Delinquency  

#### 🔁 Behavioral Analysis
- Payment history (Month_1–Month_6)
- Identified patterns of late/missed payments  

---

### 4️⃣ Pattern Identification

- Customers with high credit utilization show higher delinquency  
- High debt-to-income ratio indicates repayment risk  
- Payment behavior strongly correlates with delinquency  

---

### 5️⃣ Key Risk Indicators

| Indicator | Explanation |
|----------|------------|
| Credit Utilization | High usage indicates financial stress |
| Debt-to-Income Ratio | Higher ratio reduces repayment ability |
| Missed Payments | Strong predictor of future delinquency |
| Payment History | Repeated late/missed signals high risk |
| Loan Balance | Higher debt increases financial burden |

---

### 6️⃣ Key Insights

- Behavioral features > demographic features  
- Income alone is not a strong predictor  
- Payment history is the strongest indicator  
- Financial stress variables drive delinquency  

---

### 😲 Surprising Findings

- High-income customers can still be delinquent  
- Some customers recover despite missed payments  
- Credit behavior matters more than income  

---

## 🧹 Data Quality Summary

- Dataset is well-structured  
- Minor missing values in financial fields  
- Small categorical inconsistencies  
- Suitable for predictive modeling after cleaning  

---

## 🤖 GenAI Usage

GenAI tools were used to:
- Perform EDA efficiently  
- Detect patterns and anomalies  
- Suggest data imputation strategies  
- Generate structured reports  

---

## 💬 Detailed Prompts Used

<details>
<summary>Click to expand prompts</summary>

### 🔹 1. Initial EDA Prompt
I will upload a dataset related to customer credit behavior and delinquency risk.
Perform an Exploratory Data Analysis (EDA) and summarize the dataset.
Identify key patterns, missing values, inconsistencies, outliers, and unusual data points.
Also identify the top 3 variables most likely to predict delinquency.


---

### 🔹 2. Missing Data Handling Prompt
Analyze the dataset and identify columns with missing or inconsistent values.
Suggest the best methods to handle them (remove, mean/median imputation, predictive imputation).
Present the result in a table.


---

### 🔹 3. Relationship Analysis Prompt
Analyze relationships between variables and delinquency risk.
Identify key patterns, correlations, and high-risk indicators.
---

### 🔹 4. Summary Generation Prompt

Write a professional summary describing key patterns, data quality issues,
missing data handling, and risk indicators.
