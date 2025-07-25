# Breast Cancer Classification using Support Vector Machines (SVM)

>  Submitted by: **Tirtha Dutta**  
>  Model Type: Binary Classification | Supervised Learning  

---

##  Objective

Use Support Vector Machines (SVM) to classify breast cancer tumors as **Malignant (M)** or **Benign (B)** using the Breast Cancer Wisconsin Dataset.

---

##  Dataset Info

- **Source:** [Kaggle – Breast Cancer Dataset](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)  
- **Total Records:** 569 rows × 32 columns  
- **Target Variable:** `diagnosis` (M = Malignant, B = Benign)

---

##  What You'll Learn

- Kernel-based classification (Linear & RBF SVM)
- Feature encoding and standardization
- Hyperparameter tuning using GridSearchCV
- Visualizing decision boundaries
- End-to-end ML workflow: from raw data to results

---

##  Workflow Summary

###  1. Data Cleaning & Preprocessing  *(Proof from Task 1)*

- Dropped duplicate rows and the `id` column
- Verified missing values = 0  
- Cleaned CSV saved as:  
   `data/breast_cancer_cleaned.csv`

---

###  2. Exploratory Data Analysis *(Proof from Task 2)*

-  Boxplot of features: `images/eda_boxplot.png`  
-  Heatmap of correlations: `images/eda_heatmap.png`

---

###  3. Feature Engineering *(Proof from Tasks 1 & 6)*

- Label encoded `diagnosis`:  
  `B → 0 (Benign)` | `M → 1 (Malignant)`  
- Scaled features using `StandardScaler`

---

###  4. Model Training & Hyperparameter Tuning

- Trained **Linear SVM** and **RBF SVM**
- Used **GridSearchCV** for tuning `C` and `gamma`  
- Cross-validation (`cv=5`) accuracy: **97.89%**  
- Best parameters: `C=10`, `gamma=0.01` (RBF Kernel)

---

###  5. Task 7 – Core Proofs

|  Proof Type |  Output |
|--------------|-----------|
| Decision Boundary Plot | `images/decision_boundary.png` |
| Hyperparameter Tuning Heatmap | `images/svm_rbf_tuning_heatmap.png` |
| Classification Report | Printed in Notebook |
| Accuracy & CV Score | Printed via GridSearchCV |

---

##  Final Model Results

| Metric | Value |
|--------|-------|
| Accuracy | 97.89% |
| Kernel | RBF |
| Best `C` | 10 |
| Best `gamma` | 0.01 |

---

##  Tools & Libraries Used

- **Python 3.10+**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **scikit-learn**
- **Jupyter Notebook**

---

##  License

This project is licensed under the [MIT License](LICENSE).
