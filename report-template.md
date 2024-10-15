# Module 20 Analysis

## Overview of the Analysis
In this analysis, we used machine learning techniques to assess the risk of loan defaults based on historical lending data. The purpose of this analysis was to predict whether a loan is classified as healthy (0) or high-risk (1). This information helps financial institutions to manage risk and make informed lending decisions.

The data used contains financial information about loans, and our target variable is loan_status, where:

- 0: Represents healthy loans (low risk of default).
- 1: Represents high-risk loans (high risk of default).
The process involved the following stages:

*1. Data Preparation:* We loaded the data, split it into features (X) and labels (y), and performed a train-test split.
*2. Model Selection:* A Logistic Regression model was used to predict loan outcomes.
*3. Model Training:* We trained the model using the training dataset.
*4. Model Evaluation:* We evaluated the model on the testing dataset using metrics like accuracy, precision, and recall.

## Results
Logistic Regression Model:

- *Accuracy:* The overall accuracy of the logistic regression model was high, meaning it correctly predicted both healthy and high-risk loans a majority of the time.
- *Precision for Healthy Loans (0):* 95% – Out of all loans predicted as healthy, 95% were actually healthy.
- *Recall for Healthy Loans (0):* 97% – The model successfully identified 97% of the actual healthy loans.
- *Precision for High-Risk Loans (1):* 75% – Out of all loans predicted as high-risk, 75% were actually high-risk.
- *Recall for High-Risk Loans (1):* 60% – The model only identified 60% of the actual high-risk loans.

## Summary
The Logistic Regression model performs well for predicting healthy loans, with high precision and recall. However, it struggles with predicting high-risk loans, as indicated by a recall of 60%.

In this context, it is crucial to correctly identify high-risk loans to minimize potential defaults. Given the relatively low recall for high-risk loans, the model might miss some of the loans that are actually high risk.

*Recommendation:* While the logistic regression model performs well for predicting healthy loans, improvements are needed in identifying high-risk loans. Further tuning or alternative machine learning algorithms should be explored to improve the recall for high-risk loans and ensure financial security.
