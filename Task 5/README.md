# 🏦 Loan Eligibility Verification (Test/Evaluation Framework)

This repository holds the dedicated evaluation workflow built for handling real-world deployment challenges, featuring strict data handling rules designed for unseen testing infrastructure.

---

## 📊 Dataset Profile

* **File Name:** `test_Y3wMUE5_7gLdaTN.csv`
* **Problem Type:** Classification Evaluation (Predicting `Loan_Status`)
* **Core Objective:** Provide a robust, leak-free pipeline that reads test profiles and accurately flags structural loan eligibility.

### Features Handled
* **Applicant Demographics:** Gender, Marital Status, Dependents, Education, Self-Employment Status
* **Financial Metrics:** Applicant Income, Coapplicant Income, Loan Amount, Loan Amount Term
* **Credit Suitability:** Credit History (0.0 or 1.0), Property Area (Urban/Semiurban/Rural)

---

## 🛠️ Pipeline Architecture & Safeguards

> ⚠️ **No Data Leakage Rule:** All imputation and preprocessing techniques utilize statistics derived exclusively from the training dataset. The test set remains completely unseen until evaluation execution.

1. **Strict Imputation Logic:**
   * Missing values in categorical variables (e.g., `Gender`, `Credit_History`) are imputed using the *mode* of the training dataset.
   * Continuous missing records (`LoanAmount`) are filled utilizing training *medians*.
2. **Unified Feature Transformations:**
   * Maps out categorical components via saved encoders to ensure shape alignment matching the baseline model criteria exactly.
