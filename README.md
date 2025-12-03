# 📊 IBM HR Analytics – Employee Attrition Prediction

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML%20Models-orange.svg)
![Tableau](https://img.shields.io/badge/Tableau-Dashboard-blueviolet.svg)
![Status](https://img.shields.io/badge/Project-Completed-success.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

This project analyzes the **IBM HR Analytics Employee Attrition & Performance** dataset and builds multiple machine learning models to predict whether an employee is likely to leave the company.
It includes **data preprocessing**, **outlier handling**, **feature engineering**, **scaling**, **ML model comparison**, and a **Tableau dashboard** for visualization.

<img width="1800" height="1098" alt="Screenshot 2025-12-02 at 8 45 56 PM" src="https://github.com/user-attachments/assets/04d56a9d-55ad-4309-92aa-8f2be1a8bf7c" />


---

## 📁 Dataset

* **Source:** Kaggle – IBM HR Analytics Employee Attrition
* **Rows:** 1470
* **Columns:** 35
* **Target Variable:** `Attrition` (Yes/No)

---

# 🛠️ Project Workflow

## 1. 🔍 Data Exploration

* Inspected data types, null values, summary statistics
* Removed constant columns (`Over18`, `EmployeeCount`, `StandardHours`)
* Visualized distributions using boxplots and summary charts


## 2. ✂️ Outlier Detection & Removal

Applied **IQR (Interquartile Range)** method to detect and remove outliers across all numeric columns, resulting in a clean dataset suitable for modeling.


## 3. 🏷️ Label Encoding

Converted categorical attributes into numeric codes:

### ✔️ Binary Columns

Encoded using **LabelEncoder**
Examples:

* `Attrition`
* `Gender`
* `OverTime`

### ✔️ Multi-class Columns

Fields like `BusinessTravel`, `JobRole`, `Department`, etc., mapped to numerical values.


## 4. 📏 Feature Scaling

Used **Min-Max Scaling** to normalize all numeric columns into a **0–1** range.
Exported final dataset as `df_min_max.csv`.


## 5. 📊 Tableau Dashboard

Created interactive charts and dashboards to visualize:

* Employee demographics
* Gender balance
* Department vs role distributions
* Monthly income patterns
* Attrition insights
* Heatmaps for multi-category patterns

*[Link to the Dashboard](https://public.tableau.com/views/IBMDashboard_17647610505410/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)*


## 6. 🤖 Machine Learning Models

### 🔧 Feature Selection

Selected top-correlated features (>0.1 correlation with target).

### 🧪 Train/Test Split

80% training, 20% testing.

### 🧠 Models Implemented

* Logistic Regression
* Random Forest
* SVM
* Decision Tree
* KNN

Each evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

Compared all models visually via bar chart.
<img width="911" height="738" alt="image" src="https://github.com/user-attachments/assets/81df8dfe-c8af-4a8e-9a69-235fc5f0614a" />

---

# 📈 Results Summary

* Clear model comparison
* Visual confusion matrices
* Random Forest generally performs strongest
* Identified dominant attrition factors such as overtime, satisfaction levels, income, and tenure

---

# 🏁 Conclusion

This project delivers:

* A complete preprocessing and ML pipeline
* Feature encoding/scaling automation
* Multi-model evaluation
* HR analytics dashboard
* Practical insights to reduce employee attrition

---

# 🚀 How to Run

1. Clone repo
2. Install dependencies
3. Run notebooks
4. View Tableau dashboard

---
