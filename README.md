from pathlib import Path

readme = """# Customer Churn Prediction using Machine Learning

A machine learning project for predicting whether a telecom customer is likely to churn based on customer demographics, account information, services, contract details, and billing information.

## Project Overview

Customer churn prediction helps identify customers who may discontinue a service. This project uses the **Telco Customer Churn** dataset and applies data preprocessing, exploratory data analysis (EDA), SMOTE-based class balancing, and multiple machine learning classification models.

The notebook compares:

- Decision Tree
- Random Forest
- XGBoost

Based on the notebook's default-hyperparameter 5-fold cross-validation comparison, **Random Forest was selected for the final predictive system**.

## Dataset

The project uses:

`WA_Fn-UseC_-Telco-Customer-Churn.csv`

The dataset contains customer information such as:

- Gender
- Senior citizen status
- Partner and dependents
- Tenure
- Phone and internet services
- Online security and backup
- Device protection
- Technical support
- Streaming services
- Contract type
- Paperless billing
- Payment method
- Monthly charges
- Total charges

### Target Variable

`Churn`

- `Yes` → Customer churned
- `No` → Customer did not churn

For model training, the target is converted to:

- `1` → Churn
- `0` → No Churn

## Project Workflow

```text
Dataset
   ↓
Data Loading & Understanding
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Label Encoding
   ↓
Train-Test Split
   ↓
SMOTE for Class Balancing
   ↓
Model Training
   ├── Decision Tree
   ├── Random Forest
   └── XGBoost
   ↓
5-Fold Cross-Validation
   ↓
Random Forest Selection
   ↓
Test Set Evaluation
   ↓
Save Trained Model
   ↓
Predict Churn for New Customer Data
