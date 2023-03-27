# Module 12 Report Template

## Overview of the Analysis

In this analysis, we aimed to predict credit risk by classifying loan applicants into two categories: healthy loans (low risk) and high-risk loans (high risk). We used a dataset containing financial information about the applicants, including loan size, interest rate, income, and other relevant features. The target variable was binary, indicating whether the loan is high-risk (1) or healthy (0).

We went through several stages of the machine learning process, including data preprocessing, exploratory data analysis, feature selection, and model training and evaluation. We used the LogisticRegression classifier to build the predictive models and applied resampling techniques such as oversampling to balance the target variable's class distribution.

## Results

Using bulleted lists, we describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1 (Original Data):

Accuracy Score: 0.952
Class 0 (healthy loans) - Precision: 1.00, Recall: 0.99
Class 1 (high-risk loans) - Precision: 0.85, Recall: 0.91
Machine Learning Model 2 (Oversampled Data):

Accuracy Score: 0.9937
Class 0 (healthy loans) - Precision: 1.00, Recall: 0.99
Class 1 (high-risk loans) - Precision: 0.85, Recall: 0.91


## Summary

Based on the results, the machine learning model using oversampled data (Model 2) performs better than the model using the original data (Model 1). Model 2 has a higher balanced accuracy score (0.9937) compared to Model 1 (0.952). Precision and recall scores are also similar between the two models, but Model 2 has significantly fewer false negatives, which is crucial when identifying high-risk loans.

The performance of the models depends on the problem we are trying to solve. In this case, it is more important to predict high-risk loans (class 1) to minimize potential losses for the company. Model 2 outperforms Model 1 in this regard, as it has fewer false negatives.

We recommend using Model 2 (oversampled data) for predicting credit risk due to its superior accuracy and its ability to better identify high-risk loans. However, it's essential to be cautious when dealing with high-risk loans, as the model's performance is not as strong as it is for healthy loans. Further refinements and exploration of additional features or alternative models may improve the model's ability to predict high-risk loans more accurately.