# 📞 Bank Marketing Campaign Optimization

An end-to-end data science project predicting whether a customer will subscribe to a term deposit based on direct marketing phone campaigns. 

---

## 📊 Dataset Profile

* **File Name:** `bank.csv`
* **Problem Type:** Binary Classification (`yes` / `no`)
* **Core Objective:** Predict term deposit subscription success to optimize future marketing resource allocation and reduce cold-call fatigue.

### Key Features Analyzed
* **Client Data:** Age, Job, Marital Status, Education, Default Status, Average Yearly Balance
* **Campaign Metrics:** Contact Communication Type, Day/Month of Last Contact, Duration of Last Call
* **Past Outcomes:** Number of Contacts Performed, Days Since Last Campaign (`pdays`), Previous Campaign Outcome

---

## 🛠️ Pipeline Architecture

1. **Handling Class Imbalance:** 
   * Term deposit subscriptions are heavily imbalanced (mostly `no`). Addressed using SMOTE (Synthetic Minority Over-sampling Technique) or class weight adjustments.
2. **Feature Engineering & Transformation:**
   * Grouping sparse categorical variables (e.g., binning rare `job` types).
   * Cyclical encoding for time-based features (`month`, `day`).
3. **Model Evaluation:**
   * Focuses on the **F1-Score** and **Precision-Recall Curve** rather than simple accuracy due to the target label imbalance.
