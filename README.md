# 🚗 Car Price Prediction using Regression Models

## 📌 Project Overview

This project builds a machine learning pipeline to predict used car prices using regression techniques. It includes end-to-end steps from data preprocessing and exploratory data analysis (EDA) to model building and evaluation.

---

## 🎯 Objectives

* Predict used car prices based on vehicle features
* Identify key factors influencing price
* Handle multicollinearity and overfitting using regularization
* Compare performance of multiple regression models

---

## 📂 Dataset

* Source: AutoScout (German used car listings)
* Records: 15,915
* Features: 23
* Includes both numerical and categorical attributes such as mileage, fuel type, power, age, and features

---

## 🔍 Key Steps

### 1. Data Preprocessing

* No missing values found
* Log transformation applied to skewed target (price)
* Outlier treatment using IQR capping
* Feature scaling using StandardScaler

### 2. Feature Engineering

* Grouped low-frequency categories
* One-hot encoding for categorical variables
* Processed multi-value feature columns
* Removed multicollinearity using VIF
* Feature reduction using RFE

### 3. Exploratory Data Analysis

* Distribution analysis for numerical and categorical features
* Correlation analysis
* Identified strong predictors (hp_kW, age, km, gearing type)

---

## 🤖 Models Used

* Linear Regression (Baseline)
* Ridge Regression (L2 Regularization)
* Lasso Regression (L1 Regularization)

---

## 📊 Model Performance

| Model             | R² Score | MAE    |
| ----------------- | -------- | ------ |
| Linear Regression | ~0.93    | ~0.078 |
| Ridge Regression  | ~0.93    | ~0.079 |
| Lasso Regression  | ~0.93    | ~0.079 |

* No significant overfitting observed
* Regularization improved stability and interpretability

---

## 🔑 Key Insights

* Car model/type is the strongest price predictor
* Engine power (hp), age, and mileage significantly impact price
* Transmission and added features (LED lights, parking sensors) influence pricing
* Linear models are sufficient for this dataset

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

## 🚀 Future Improvements

* Try ensemble models (Random Forest, XGBoost)
* Advanced feature engineering
* Deploy model as API or web app

---

## 📎 Conclusion

This project demonstrates a complete regression workflow and shows that well-preprocessed structured data can achieve high accuracy with simple linear models.

---

## 👤 Author

Omkar Kadam
