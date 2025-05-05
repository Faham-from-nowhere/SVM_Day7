# 🔍 SVM Classification on Breast Cancer Dataset

This project demonstrates how to apply **Support Vector Machines (SVM)** for binary classification using the popular **Breast Cancer Wisconsin** dataset. The key objectives include data preparation, model training using different SVM kernels, hyperparameter tuning, decision boundary visualization, and performance evaluation using cross-validation.

---

## 📁 Project Structure

SVM_BreastCancer/
├── svm_breast_cancer.ipynb # Main Jupyter notebook
├── README.md # This file



---

## 📌 Objectives

1. ✅ Load and prepare a dataset for binary classification  
2. ✅ Train an SVM using **Linear** and **RBF** kernels  
3. ✅ Visualize the **decision boundary** using 2D PCA  
4. ✅ Perform **hyperparameter tuning** using GridSearchCV (`C`, `gamma`)  
5. ✅ Evaluate the model using **cross-validation** and performance metrics  

---

## 📊 Dataset Used

- **Name:** Breast Cancer Wisconsin (Diagnostic)
- **Source:** `sklearn.datasets.load_breast_cancer()`
- **Type:** Binary classification (Malignant vs. Benign)
- **Features:** 30 numerical attributes related to cell nuclei

---

## 🧠 Techniques Applied

- **Standardization** using `StandardScaler`
- **Support Vector Machines (SVC)** with Linear, RBF, and Polynomial kernels
- **Hyperparameter Tuning** using `GridSearchCV`
- **Cross-Validation** to evaluate model performance
- **Dimensionality Reduction** with `PCA` for visualization
- **Decision Boundary Plotting** with `mlxtend`

---

## ✅ Model Evaluation Summary

### 📌 Linear SVM
- **Test Accuracy:** 95.61%
- **Precision (Class 0):** 93%
- **Recall (Class 0):** 95%
- **Precision (Class 1):** 97%
- **Recall (Class 1):** 96%
- **F1-Score (Weighted):** 96%

---

### 📌 RBF SVM (Untuned)
- **Test Accuracy:** 98.25%
- **Precision (Class 0):** 100%
- **Recall (Class 0):** 95%
- **Precision (Class 1):** 97%
- **Recall (Class 1):** 100%
- **F1-Score (Weighted):** 98%

---

### 📌 RBF SVM (After GridSearchCV Tuning)
- **Best Parameters:** `C = 100`, `gamma = 0.001`
- **Best Cross-Validation Accuracy:** **97.36%**
- **Test Accuracy with Best Parameters:** **98.25%**
- **F1-Score (Weighted):** 98%

#### 🔁 Cross-Validation Scores:
[0.978, 0.967, 1.000, 0.978, 0.945]
Mean CV Accuracy: 97.36%

