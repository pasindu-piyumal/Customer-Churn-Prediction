# Customer Churn Prediction

A machine learning project for predicting customer churn using the Telco Customer Churn dataset. The project explores customer behavior, performs data preprocessing and feature engineering, handles class imbalance using SMOTE, and compares multiple machine learning classification models.

---

## 📌 Project Overview

Customer churn refers to the situation where customers stop using a company's products or services.

Predicting churn can help organizations:

- Identify customers who are likely to leave
- Understand important factors associated with churn
- Develop customer retention strategies
- Prioritize high-risk customers
- Improve customer relationship management

This project develops and evaluates machine learning models to predict whether a customer is likely to churn.

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze customer demographic and service-related information.
2. Clean and preprocess the raw customer dataset.
3. Investigate missing values and potential outliers.
4. Engineer meaningful features using feature binning.
5. Encode categorical variables.
6. Scale numerical features.
7. Handle class imbalance using SMOTE.
8. Train multiple machine learning classification models.
9. Perform hyperparameter tuning using GridSearchCV.
10. Evaluate models using multiple classification metrics.
11. Identify the best-performing model for churn prediction.

---

## 📊 Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information related to:

- Demographics
- Customer tenure
- Phone services
- Internet services
- Online security
- Technical support
- Streaming services
- Contract information
- Payment methods
- Monthly charges
- Total charges
- Customer churn

### Dataset Size

| Description | Value |
|---|---:|
| Original records | 7,043 |
| Records after preprocessing | 7,032 |
| Original features | 21 |
| Target variable | Churn |

### Target Distribution

| Churn | Count | Percentage |
|---|---:|---:|
| No | 5,174 | 73.46% |
| Yes | 1,869 | 26.54% |

The dataset is therefore imbalanced, making metrics such as Precision, Recall, F1-score, ROC-AUC and PR-AUC important.

---

## 🔄 Machine Learning Workflow

```text
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Missing Value Handling
     │
     ▼
Exploratory Analysis
     │
     ▼
Outlier Investigation
     │
     ▼
Feature Engineering
     │
     ▼
Feature Binning
     │
     ▼
Train/Test Split
     │
     ▼
Categorical Encoding
     │
     ▼
Numerical Scaling
     │
     ▼
SMOTE
     │
     ▼
Hyperparameter Tuning
     │
     ├───────────────┐
     ▼               ▼
Logistic        Decision Tree
Regression
     │               │
     └───────┬───────┘
             ▼
       Random Forest
             │
             ▼
       Model Evaluation