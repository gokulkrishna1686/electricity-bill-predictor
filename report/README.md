# Gokul Krishna Balaji, CS24B2053 – Electricity Bill Predictor

## Overview

This project was built for the AI & ML Hackathon at IIITDM Kancheepuram. The goal is to build a supervised regression model that accurately predicts a household's monthly electricity bill using appliance usage data, city, company, tariff rate, and more.

The model helps simulate how utility providers can forecast energy costs and detect anomalies in billing.

---

## Problem Statement

> Predict the `ElectricityBill` for a given household based on features such as:
- Number of appliances (Fan, Refrigerator, Air Conditioner, etc.)
- Monthly usage hours
- Tariff rate
- City and Company (categorical data)

---

## Tools & Libraries Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook (Google Colab)

---

## Preprocessing Steps

- One-hot encoding for `City` and `Company` (categorical features)
- Scaling numerical features using `RobustScaler` to handle outliers
- Outlier detection and removal for scaled data (optional experiment)
- Train-test split (80/20)

---

## Models Tried

- Linear Regression  
- Random Forest Regressor (with hyperparameter tuning using `n_estimators`)

We compared models across different versions of the dataset:
- Unscaled
- Scaled
- Scaled with outliers removed

---

## Results Summary

Random Forest with `n_estimators=300` on the **scaled dataset (with outliers included)** gave the best performance:

- **RMSE**: 0.003489  
- **R² Score**: 0.999977

--- 

## Demo Video

You can find a short 2–3 minute video explaining the approach and results here:

[Click to watch demo video](video/demo_video.mp4)

---