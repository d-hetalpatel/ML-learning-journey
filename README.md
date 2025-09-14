# 🧠 Support Vector Machine (SVM) with Scikit-Learn

This repository contains Jupyter notebooks demonstrating the use of **Support Vector Machines (SVM)** for both **classification** and **regression** tasks.

---

## 📂 Notebooks

1. **SVM_Classification.ipynb**  
   - Dataset: **Breast Cancer (Scikit-learn)**  
   - Task: Classify tumors as **benign (1)** or **malignant (0)**  
   - Techniques:  
     - GridSearchCV for hyperparameter tuning  
     - Confusion Matrix visualization  
     - Classification Report (precision, recall, F1-score)  

2. **SVM_Regression.ipynb**  
   - Dataset: **California Housing (Scikit-learn)**  
   - Task: Predict **median house values**  
   - Techniques:  
     - Standardization of features (StandardScaler)  
     - GridSearchCV for hyperparameter tuning  
     - Evaluation with **Root Mean Squared Error (RMSE)**  
     - Actual vs Predicted scatter plot  

---

## Key Concepts

- **Support Vector Machine (SVM):** Supervised learning algorithm that finds an optimal hyperplane for classification or regression.  
- **Kernel Trick:** Allows handling of non-linear data by projecting it into higher dimensions (e.g., RBF kernel).  
- **GridSearchCV:** Automated hyperparameter tuning using cross-validation.  

---

## Results Summary

| Task           | Metric                 | Performance (approx.) |
|----------------|------------------------|------------------------|
| Classification | Accuracy               | ~90–95%                |
| Regression     | RMSE (lower is better) | Reasonable (varies)    |

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/SVM-Classification-Regression.git
