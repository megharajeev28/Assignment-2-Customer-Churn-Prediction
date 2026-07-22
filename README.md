# CUSTOMER CHURN PREDICTION USING LOGISTIC REGRESSION

## ASSIGNMENT – 2

---

## STUDENT DETAILS

| Field | Details |
|--------|---------|
| **AUTHOR** | Megha Rajeev |
| **REGISTRATION NUMBER** | 23MIM10047 |
| **APPLICATION NUMBER** | IN26011193 |
| **BATCH NUMBER** | 1A |
| **EMAIL ID** | megha.23mim10047@vitbhopal.ac.in |

---

## OBJECTIVE

The objective of this project is to develop a **Logistic Regression** model capable of predicting whether a telecommunications customer is likely to churn based on demographic information, subscribed services, and billing details. The project demonstrates the complete machine learning workflow, including data understanding, exploratory data analysis, preprocessing, model development, and performance evaluation.

---

## DATASET

**Dataset Name:** Telco Customer Churn Dataset

**Kaggle Link:**
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

> **Note:** The dataset is not included in this repository. Please download it directly from Kaggle using the link above.

---

## PROBLEM STATEMENT

A telecommunications company wants to predict whether a customer is likely to leave (churn) based on demographic information and service usage.

The objective is to build a **Logistic Regression** model that accurately classifies customers into:

- **No Churn (0)**
- **Churn (1)**

---

## LIBRARIES USED

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## METHODOLOGY

### 1. DATA LOADING

- Loaded the Telco Customer Churn dataset using Pandas.

### 2. DATA UNDERSTANDING

- Explored dataset structure.
- Identified numerical and categorical features.
- Examined the target variable.
- Checked for missing values and duplicate records.

### 3. EXPLORATORY DATA ANALYSIS (EDA)

- Customer Churn Distribution
- Numerical Feature Distributions
- Categorical Feature Analysis
- Relationship between Features and Churn
- Correlation Heatmap

### 4. DATA PREPROCESSING

- Removed unnecessary columns (`customerID`)
- Converted `TotalCharges` to numeric format
- Handled missing values
- Encoded the target variable (`Churn`)
- Applied **One-Hot Encoding** to categorical features
- Performed **80:20 Stratified Train-Test Split**
- Standardized numerical features using **StandardScaler**

### 5. MODEL DEVELOPMENT

- Built a **Logistic Regression** classifier
- Trained the model using the training dataset
- Predicted customer churn on the testing dataset

### 6. MODEL EVALUATION

The model was evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC Score
- Classification Report

---

## RESULTS

| Metric | Value |
|---------|-------|
| **Accuracy Score** | **79.84%** |
| **Precision** | **63.98%** |
| **Recall** | **55.08%** |
| **F1-Score** | **59.20%** |
| **ROC-AUC Score** | **0.8409** |

### Confusion Matrix

| | Predicted: No Churn | Predicted: Churn |
|---|---:|---:|
| **Actual: No Churn** | 919 | 116 |
| **Actual: Churn** | 168 | 206 |

---

## KEY FINDINGS

- Customers with **month-to-month contracts**, **higher monthly charges**, and **shorter tenure** are more likely to churn.
- Contract type, internet service, payment method, and tenure significantly influence customer churn.
- Logistic Regression achieved good classification performance and serves as a strong baseline model for churn prediction.

---

## CONCLUSION

This project successfully developed a **Logistic Regression** model to predict customer churn using demographic, service usage, and billing information from the Telco Customer Churn dataset. The model achieved an **Accuracy Score of 79.84%**, demonstrating good predictive performance in identifying customers who are likely to leave the company. Exploratory Data Analysis showed that factors such as **contract type, tenure, monthly charges, internet service, and payment method** have a significant influence on customer churn. Customers with shorter tenure and month-to-month contracts were found to have a higher likelihood of churning. Although the model performed well, **Logistic Regression assumes a linear relationship between the features and the log-odds of the target variable**, which may limit its ability to capture complex nonlinear patterns. More advanced machine learning models could further improve prediction performance.

---

## PROJECT STRUCTURE

```
Customer-Churn-Prediction-Using-Logistic-Regression
│
├── Assignment-2.ipynb
├── README.md
```

---

## AUTHOR

**Megha Rajeev**

Integrated M.Tech in Artificial Intelligence

VIT Bhopal University
