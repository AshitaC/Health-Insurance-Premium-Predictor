# Health-Insurance-Premium-Predictor

## Overview

This project aims to predict insurance premium amounts based on various demographic and health-related factors. It utilizes **Linear Regression, Ridge Regression, and XGBoost Regressor** , with XGBoost achieving the best performance.

## Dataset

The dataset includes the following features:

Demographics: Age, Gender, Region, Marital Status, Number of Dependents

Health Factors: BMI Category, Smoking Status, Medical History (risk score)

Employment & Income: Employment Status, Income Level (Lakhs)

Insurance Details: Insurance Plan, Annual Premium Amount (Target Variable)

## Model Performance

| Model |  Linear Regression  | Ridge Regression | XGBoost Regression |
|:-----|:--------:|------:|------:|
| MSE   | 5165611 | 5165652 | 1574451 |
| RMSE   |  2272  |   2272 |   **1254** |
| R2   |0.92 |    0.92 |  **0.98** |


**XGBoost** significantly outperforms other models, achieving the lowest RMSE.

# Feature Engineering

Encoded categorical variables (One-Hot Encoding & Label Encoding)

Created a risk score for medical conditions

Normalized the risk score for better model interpretability.

Feature Importance (XGBoost)

# Key Findings:

- _Insurance Plan_ and _Age_ are the most influential factors in predicting premium amounts.

- Other contributing factors include BMI category (Obesity, Overweight), Risk Score, and Smoking Status.

# Technologies Used

- Python (pandas, numpy, scikit-learn, XGBoost, Statsmodels)

- Matplotlib & Seaborn (for data visualization)
