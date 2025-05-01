
# 🌳 Task 5: Decision Trees and Random Forests

## 📌 Objective
The goal of this task is to explore and implement tree-based machine learning models—specifically **Decision Trees** and **Random Forests**—for classification problems. The project demonstrates how to train, visualize, and evaluate these models while also addressing overfitting and model interpretability.

---

## 📁 Dataset

- **Name**: Heart Disease Dataset
- **Format**: CSV
- **Shape**: 302 rows × 12 columns
- **Target Variable**: `target` (0 = No Disease, 1 = Disease)

---

## 🛠 Tools and Libraries Used

- Python
- Scikit-learn (for modeling and evaluation)
- Graphviz (for decision tree visualization)
- Pandas & NumPy (for data manipulation)
- Seaborn & Matplotlib (for plotting and insights)

---

## 🧠 Theoretical Background

### 🌲 Decision Trees

A **Decision Tree** is a flowchart-like structure used for classification or regression. It splits the dataset into subsets using feature values that offer the highest *information gain* or lowest *Gini impurity*.

#### Key Concepts:

- **Entropy**: Measures impurity in a dataset. High entropy = high disorder.
- **Information Gain**: Reduction in entropy after a dataset split.
- **Gini Index**: Alternative to entropy, measures impurity more efficiently.
- **Overfitting**: Trees may learn noise. Controlled by parameters like `max_depth`, `min_samples_split`, etc.

### 🌲🌲 Random Forests

A **Random Forest** is an ensemble of Decision Trees trained on random subsets of the dataset using **Bagging (Bootstrap Aggregating)**.

#### Advantages:

- Reduces overfitting
- Improves accuracy and robustness
- Handles high-dimensional spaces well

---

## 📊 Model Implementation Summary

### ✅ Decision Tree Classifier

- Trained using Gini criterion
- Controlled tree complexity using:
  - `max_depth`
  - `min_samples_split`
  - `min_samples_leaf`
- Tree visualized using Graphviz (`export_graphviz` + `.render()`)
- Feature importances plotted to understand influence on predictions

### ✅ Random Forest Classifier

- Aggregates multiple trees for improved accuracy and stability
- Provides feature importance ranking
- Outperforms individual Decision Tree in generalization

---

## 📈 Evaluation Metrics

### ⚙️ Confusion Matrix Summary

| Predicted / Actual | No Disease | Disease |
|--------------------|------------|---------|
| **No Disease**     | 96         | 0       |
| **Disease**        | 0          | 109     |

### ✔ Classification Report

| Class        | Precision | Recall | F1-score | Support |
|--------------|-----------|--------|----------|---------|
| No Disease   | 1.00      | 1.00   | 1.00     | 96      |
| Disease      | 1.00      | 1.00   | 1.00     | 109     |
| **Accuracy** |           |        | **1.00** | 205     |


### Accuracy

- **Train Accuracy**: 100%
- **Test Accuracy**: 100%

### 🔁 Cross-Validation Score

- **Mean Accuracy**: 0.993
- **Standard Deviation**: ±0.009

---

### Feature Importance (Top Predictors)
- `cp` (chest pain type)
- `thalach` (max heart rate)
- `oldpeak` (ST depression)

---

## 🔍 Visualizations Used

- 📊 Decision Tree (Graphviz plot)
- 📉 Feature Importance (Bar Plot)
- ✅ Confusion Matrix (Heatmap)
- 📌 Evaluation Metrics Table

---


## 🧾 Instructions to Run

3. Open `Task5.ipynb` using Jupyter Notebook or Google Colab.
4. Follow the sections for data preprocessing, training, evaluation, and visualization.

---

## 📎 Download

This repository contains a complete Jupyter Notebook (`Task5.ipynb`) with all outputs, visualizations, and analysis steps embedded. No external dependencies are needed apart from the usual data science stack.

---

