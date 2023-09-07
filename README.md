# Module 12 Report: Machine Learning Model Analysis

## Overview of the Analysis
The purpose of this analysis is to develop and evaluate machine learning models for predicting loan risk. The analysis aims to assist in making informed decisions regarding loan approvals based on financial information provided.The dataset used for this analysis contains various financial attributes related to loan applications, including loan size, interest rate, borrower income, debt-to-income ratio, the number of accounts, derogatory marks, and total debt. The aim is to predict the loan's risk level, which is represented by the binary variable "loan_status," where "0" indicates a healthy loan and "1" signifies a high-risk loan.

### Variables and Value Counts
This is the value counts for each variables:

- Healthy Loans (0): Count = 75,036
- High-Risk Loans (1): Count = 2,500

### Stages of the Machine Learning Process
In the analysis We have gone through different stages like:

1. **Data Preprocessing**: We loaded the dataset, split it into features and labels, and addressed class imbalance.
2. **Model Building**: We trained logistic regression models using both the original and resampled datasets.
3. **Model Evaluation**: We calculated various metrics, including accuracy, balanced accuracy, precision, recall, F1-score, and generated confusion matrices.
4. **Comparison**: We compared model performance to make recommendations.


### Methods Used
- Logistic Regression: We used for building and training the classification models.
- RandomOverSampler: We applied to address class imbalance by resampling the data

## Results

### Machine Learning Model 1

- Balanced Accuracy Score: 0.952 (Original Data) -> For the original data, the balanced accuracy score is 0.952, indicating that the model, on average, correctly predicts 95.2% of the samples from both classes.
- Precision (High-Risk Loans): 0.85 (Original Data) -> For the original data, the precision for high-risk loans is 0.85, meaning that when the model predicts a loan as high-risk, it is correct 85% of the time.
- Recall (High-Risk Loans): 0.91 (Original Data) ->  For the original data, the recall for high-risk loans is 0.91, meaning that the model correctly identifies 91% of all actual high-risk loans.

### Machine Learning Model 2

- Balanced Accuracy Score:  0.994 (Resampled Data) -> For the resampled data, the balanced accuracy score is 0.994, indicating that the model, on average, correctly predicts 99.4% of the samples from both classes. 
- Precision (High-Risk Loans): 0.84 (Resampled Data) -> For the resampled data, the precision for high-risk loans is 0.84, indicating that when the model predicts a loan as high-risk, it is correct 84% of the time.
- Recall (High-Risk Loans):  0.99 (Resampled Data) -> For the resampled data, the recall for high-risk loans is 0.99, indicating that the model correctly identifies 99% of all actual high-risk loans.

This suggests that the model trained on resampled data is better at capturing high-risk loans.

## Summary

Both models performed well, with the resampled data consistently outperforming the original data. We recommend using the resampled logistic regression model, especially for identifying high-risk loans. In summary, the resampled logistic regression model is our preferred choice for predicting loan risk due to its strong performance, especially in identifying high-risk loans. However, both models provide valuable insights.
