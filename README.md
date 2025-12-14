# Telco Customer Churn Prediction

## Overview

This repository contains my final project for DATA 1030.  
The goal is to build and interpret a machine learning model that predicts whether a telecom customer will churn (leave the service). I focus on a full supervised-learning pipeline: preprocessing, 
model training with cross-validation, uncertainty estimation, and model interpretability with global and local feature importance (SHAP).

## Dataset

The project uses the public **IBM Telco Customer Churn** dataset from Kaggle:

- Source: https://www.kaggle.com/datasets/blastchar/telco-customer-churn  
- Task: binary classification (`Churn` = “Yes” / “No”)  
- Features: customer demographics, contract type, payment method, monthly and total charges, and subscriptions to various services.

## Environment and Reproducibility

The code was developed and tested with the following software versions:

- Python 3.10  
- numpy 1.26.x  
- pandas 2.2.x  
- scikit-learn 1.4.x  
- matplotlib 3.8.x  
- seaborn 0.13.x  
- xgboost 2.0.x  
- shap 0.45.x


---

Save this as `environment.yml` :

```yaml
name: data1030-project
channels:
  - defaults
dependencies:
  - python=3.10
  - numpy=1.26
  - pandas=2.2
  - scikit-learn=1.4
  - matplotlib=3.8
  - seaborn=0.13
  - pip
  - pip:
      - xgboost==2.0.3
      - shap==0.45.0
