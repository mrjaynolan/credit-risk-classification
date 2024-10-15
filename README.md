# credit-risk-classification
Module 20 Challenge

This project applies a Logistic Regression model to predict the likelihood of loan defaults (high-risk loans) using historical lending data. The goal is to classify loans as either healthy or high-risk based on the features in the dataset.

## Project Steps

### 1. Data Loading and Preparation:
    - The lending data is loaded from lending_data.csv.
    - The target variable (y) is set as loan_status, where 0 represents healthy loans and 1 represents high-risk loans.
    - The remaining columns are used as features (X).
    - The dataset is split into training and testing sets.
### 2. Logistic Regression Model:
    - A logistic regression model is trained using the training dataset.
    - Predictions are made on the testing dataset.
    - Model performance is evaluated using a confusion matrix and classification report.
### 3. Model Evaluation:
    - Accuracy, precision, recall, and F1-score metrics are used to assess the model’s ability to predict both healthy and high-risk loans.
 
 ## Results

  - Accuracy: The model achieved a high overall accuracy in classifying loans.
  - Precision for Healthy Loans (0): 95%
  - Recall for Healthy Loans (0): 97%
  - Precision for High-Risk Loans (1): 75%
  - Recall for High-Risk Loans (1): 60%

## Summary

The logistic regression model is effective at identifying healthy loans, with high precision and recall. However, its ability to detect high-risk loans is weaker, with lower recall (60%), meaning it misses a significant number of risky loans. Due to this limitation, the model may need further tuning or an alternative approach to improve the detection of high-risk loans.
