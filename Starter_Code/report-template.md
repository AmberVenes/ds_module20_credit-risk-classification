# Module 12 Report Template

## Overview of the Analysis

Purpose of the Analysis
The aim of this analysis is to determine whether the Logistic Regression machine learning model can more effectively predict healthy loans versus high-risk loans by using either the original dataset or a resampled dataset to increase the representation of the minority class.

The Dataset
The dataset used for this analysis contains information on 77,536 loans. It includes variables such as loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derogatory_marks, total_debt, and loan_status. The target variable we aim to predict is loan_status, while the other columns serve as features to train the model and guide its predictions.

Machine Learning Process Steps
The machine learning process involves several steps to ensure the model works well. These steps are:

Data Preparation – Import the dataset, create a DataFrame, and check the columns and features.
Separate Features and Labels – Split the data into features (input) and labels (target: loan status as healthy (0) or high-risk (1)).
Train-Test Split – Use the train_test_split function to split the data into training and testing sets.
Import the Model – Load the LogisticRegression model from SKLearn.
Instantiate the Model – Create an instance of the logistic regression model.
Train the Model – Fit the model to the training data.
Make Predictions – Use the trained model to predict outcomes on the test data.
Evaluate Results – Measure the model's accuracy with metrics like accuracy score, confusion matrix, and classification report.

Machine Learning Methods Used
For this analysis, the primary model employed is:

LogisticRegression from SKLearn

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Key performance metrics of the Logistic Regression model are listed below:

Accuracy: 0.99
Precision:
Class 0: 1.00
Class 1: 0.85
Recall:
Class 0: 0.99
Class 1: 0.91

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

*In the end, the Logistic Regression model performed extremely well, especially in predicting Class 0 (healthy loans), with near-perfect precision and recall. For Class 1 (high-risk loans), the model showed a precision of 0.85 and a recall of 0.91, meaning it was more likely to predict false positives than false negatives. Overall, the model demonstrated strong predictive power for both loan categories, but additional testing on other datasets is recommended before using the model for actual loan predictions.