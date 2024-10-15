# **Module 20 Analysis**

## **Overview of the Analysis**
In this analysis, we used machine learning techniques to assess the risk of **loan defaults** based on historical lending data. The objective was to predict whether a loan is classified as **healthy (0)** or **high-risk (1)**. This information is valuable for financial institutions to manage loan portfolios and mitigate risk effectively.

The data contains various financial features about loans, with the target variable being `loan_status`, where:
- **0**: Represents **healthy loans** (low risk of default).
- **1**: Represents **high-risk loans** (high risk of default).

### **Steps in the Process**:
1. **Data Preparation**: Loaded the data, split it into features (`X`) and labels (`y`), and divided it into training and testing datasets.
2. **Model Selection**: We applied a **Logistic Regression** model to predict the loan outcomes.
3. **Model Training**: Trained the model using the training data (`X_train` and `y_train`).
4. **Model Evaluation**: Assessed the model using accuracy, precision, recall, and other performance metrics on the test data.

---

## **Results**
### **Logistic Regression Model**:

- **Accuracy**: The logistic regression model achieved a high overall accuracy, indicating it correctly predicted both healthy and high-risk loans a majority of the time.
- **Precision for Healthy Loans (0)**: **95%** – Out of all the loans predicted as healthy, 95% were actually healthy.
- **Recall for Healthy Loans (0)**: **97%** – The model successfully identified 97% of the actual healthy loans.
- **Precision for High-Risk Loans (1)**: **75%** – Out of all the loans predicted as high-risk, 75% were indeed high-risk.
- **Recall for High-Risk Loans (1)**: **60%** – The model correctly identified only 60% of the actual high-risk loans.

---

## **Summary**
The **Logistic Regression model** performs well in predicting **healthy loans** with high precision and recall. However, the model's performance in predicting **high-risk loans** is less effective, with a recall of only **60%**, meaning it fails to identify a significant portion of the high-risk loans.

### **Recommendation**:
While the model is reliable for predicting healthy loans, it needs improvement in detecting high-risk loans to minimize potential defaults. Further tuning of the model or exploring alternative machine learning algorithms is recommended to improve recall for high-risk loans, ensuring better risk management for financial institutions.

