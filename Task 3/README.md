# 💸 Medical Insurance Cost Estimation

This regression project investigates how individual demographic and lifestyle factors affect annual medical insurance charges. The finalized model allows for accurate premium forecasting based on user profiles.

---

## 📊 Dataset Profile

* **File Name:** `insurance.csv`
* **Problem Type:** Regression
* **Core Objective:** Predict individual insurance costs (`charges`) accurately, minimizing Root Mean Squared Error (RMSE).

### Key Features Analyzed
* **Numerical:** `age`, `bmi` (Body Mass Index), `children` (number of dependents)
* **Categorical:** `sex`, `smoker` (yes/no status), `region` (US geographic quadrants)

---

## 🛠️ Pipeline Architecture

1. **Exploratory Data Analysis:**
   * Segmenting variables to uncover trends.
   * *Crucial Visualization:* Scatter plots of `age` vs `charges` segmented by `smoker` status reveal clean linear trajectories.
2. **Feature Preprocessing:**
   * Transforming categorical entries via `pd.get_dummies()`.
   * Log-transforming the target variable `charges` to normalize its right-skewed distribution.
3. **Algorithms Evaluated:**
   * Linear Regression (Baseline), Ridge/Lasso regularization, and Gradient Boosting Regressor.
