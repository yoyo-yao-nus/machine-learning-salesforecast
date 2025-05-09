# 🛒 Sales Forecasting and Inventory Optimization System

**Tags:** `Machine Learning` `Regression Modeling` `Gradient Boosting` `Inventory Management` `Python`

## 📌 Project Overview
This project supports intelligent inventory decisions for e-commerce businesses by forecasting sales using machine learning models and optimizing inventory decisions using the Newsvendor model.

> 💡 Independently completed end-to-end: data preprocessing, modeling, evaluation, and decision optimization.

---

## 🔧 Technologies Used
- **Programming:** Python, Pandas, NumPy, Matplotlib
- **Modeling:** Scikit-learn (Linear Regression, Lasso, Ridge, Gradient Boosting, Random Forest)
- **Validation:** K-Fold Cross Validation, Residual Analysis
- **Optimization:** Empirical Distribution, Newsvendor Inventory Theory

---

## 📈 Key Features

### 🔍 1. Data Exploration & Feature Engineering
- Analyzed and cleaned e-commerce sales data.
- Identified key predictors like `clickVolume`, `avgFinalUnitPrice`, and `ma14SalesVolume`.
- Applied logarithmic transformations for normalization.

### 📊 2. Predictive Modeling
- Built and evaluated multiple models:
  - Linear Regression with interaction and polynomial terms
  - Regularized models (Lasso and Ridge)
  - Ensemble methods: Gradient Boosting and Random Forest

- **Best Model:** Gradient Boosting with:
```python
learning_rate = 0.3
n_estimators = 200
max_depth = 3
```
- Achieved cross-validated MSE: **≈ 866**

### 📦 3. Inventory Decision Modeling
- Used the **Newsvendor model** to optimize stock levels and maximize profit.
- Estimated sales uncertainty using empirical distribution of residuals.
- Adjusted predictions to compute the profit-maximizing inventory quantity:
```math
y* = predicted_sales + ε*
where ε* = inverse CDF at underage ratio (e.g. 2/3)
```

---

## ✅ Results
- Achieved high accuracy in sales prediction (MSE significantly reduced).
- Integrated economic theory into machine learning workflow.
- Provided a scalable solution for inventory management in e-commerce.

---

## 📁 Folder Structure (Optional)
```bash
project/
├── data/
│   ├── train.csv
│   ├── test.csv
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_RegressionModels.ipynb
│   ├── 03_Boosting_RF.ipynb
│   └── 04_InventoryDecision.ipynb
├── models/
│   └── final_boosting_model.pkl
├── results/
│   └── predictions.csv
├── README.md
```

---

## 📬 Contact
If you'd like to learn more or discuss this project, feel free to reach out via GitHub or email.
