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

- Balanced Accuracy Score: 0.952 (Original Data) / 0.994 (Resampled Data)
- Precision (High-Risk Loans): 0.85 (Original Data) / 0.84 (Resampled Data)
- Recall (High-Risk Loans): 0.91 (Original Data) / 0.99 (Resampled Data)

### Machine Learning Model 2

- Balanced Accuracy Score: 0.952 (Original Data) / 0.994 (Resampled Data)
- Precision (High-Risk Loans): 0.85 (Original Data) / 0.84 (Resampled Data)
- Recall (High-Risk Loans): 0.91 (Original Data) / 0.99 (Resampled Data)

## Summary

Both models performed well, with the resampled data consistently outperforming the original data. We recommend using the resampled logistic regression model, especially for identifying high-risk loans.

- **Performance Dependence**: The choice of model may depend on specific goals. The resampled model is better for high-risk loan prediction, while both models work well for balanced predictions.

- **No Model Rejection**: Both models are valid options, and the choice should align with your institution's objectives.

In summary, the resampled logistic regression model is our preferred choice for predicting loan risk due to its strong performance, especially in identifying high-risk loans. However, both models provide valuable insights.
