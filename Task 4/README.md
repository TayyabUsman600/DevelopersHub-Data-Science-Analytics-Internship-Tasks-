# 🌸 Iris Species Classification

The classic introductory machine learning project implementing multi-class classification to accurately categorize Iris flowers into three distinct species based on geometric structural measurements.

---

## 📊 Dataset Profile

* **File Name:** `iris.csv`
* **Problem Type:** Multi-class Classification (3 Classes)
* **Target Classes:** *Iris setosa*, *Iris versicolor*, *Iris virginica*

### Structural Features
* Petal Length & Petal Width
* Sepal Length & Sepal Width

---

## 🛠️ Pipeline Architecture

1. **Pairplot Analysis:**
   * Generated comprehensive pairwise scatter plots using `sns.pairplot(hue='species')` to show clean structural clusters. *Iris setosa* is perfectly linearly separable from the other two species.
2. **Modeling & Training:**
   * Split data using `train_test_split(X, y, test_size=0.2, random_state=42)`.
   * Standardized classification using Support Vector Machines (SVM), Decision Trees, and Random Forests.
3. **Metrics:**
   * Evaluated via Macro/Weighted Accuracy, Precision, Recall, and a clean Confusion Matrix plot.
