# 🏦 Bank Customer Churn Prediction

This project focuses on predicting customer attrition using machine learning. By analyzing historical customer demographics, account statuses, and activity metrics, the model identifies individuals at high risk of leaving the bank, enabling proactive retention strategies.

---

## 📊 Dataset Profile

* **File Name:** `Bank Customer Churn Prediction.csv`
* **Problem Type:** Binary Classification (`1` = Churned, `0` = Retained)
* **Core Objective:** Maximize recall to capture as many churn-prone customers as possible while maintaining balanced precision.

### Key Features Analyzed
* **Demographics:** Age, Gender, Geography
* **Financial Metrics:** Credit Score, Account Balance, Estimated Salary
* **Account Status:** Tenure, Number of Products, Has Credit Card (`HasCrCard`), Is Active Member (`IsActiveMember`)

---

## 🛠️ Pipeline Architecture

1. **Exploratory Data Analysis (EDA):**
   * Visualizing numerical distributions using `sns.boxplot` and `sns.histplot`.
   * Analyzing correlation matrices to pinpoint strong indicators of churn (e.g., Age and Activity status).
2. **Data Preprocessing:**
   * One-Hot Encoding for categorical features (`Geography`, `Gender`).
   * Feature scaling (Standardization) for skewed numerical data like `Balance` and `EstimatedSalary`.
3. **Model Selection & Evaluation:**
   * Baseline models implemented: Logistic Regression, Random Forest, and XGBoost.
   * Evaluated using Confusion Matrices, ROC-AUC curves, and Classification Reports.

---

## 📈 Key Insights Summary
* **Age vs. Churn:** Older customers tend to exhibit a significantly higher churn rate compared to younger demographics.
* **Product Density:** Customers holding more than two bank products show an exponential increase in attrition probability.
