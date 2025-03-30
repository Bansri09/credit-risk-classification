# Credit Risk Analysis Challenge

This challenge involves building and evaluating a machine learning model to predict loan risk based on historical lending data. The dataset comes from a peer-to-peer lending service, and the goal is to use the dataset to classify loans as either healthy (low-risk) or high-risk based on the creditworthiness of borrowers.

## Challenge Overview

The objective of this challenge is to train a logistic regression model using historical lending activity and evaluate the model’s performance in identifying high-risk loans. The final goal is to generate a comprehensive analysis of the model's performance, along with a credit risk report suitable for use in a loan approval system.

## Challenge Steps

### 1. Split the Data into Training and Testing Sets

- **Data Loading**: The dataset (`lending_data.csv`) should be loaded into a Pandas DataFrame from the `Resources` folder.
- **Data Preprocessing**:
  - Extract the labels (y) from the `loan_status` column (0 = healthy loan, 1 = high-risk loan).
  - Create the feature set (X) from the remaining columns.
- **Data Splitting**: Use `train_test_split` to divide the dataset into training and testing sets.

### 2. Create a Logistic Regression Model with the Original Data

- **Model Training**: Fit a logistic regression model using the training data (`X_train`, `y_train`).
- **Model Prediction**: Use the fitted model to make predictions on the testing data (`X_test`).
- **Model Evaluation**: 
  - Generate a confusion matrix to assess the model’s performance.
  - Print a classification report to evaluate precision, recall, and F1-score for both healthy and high-risk loan predictions.

### 3. Write a Credit Risk Analysis Report

- **Overview**: Provide an explanation of the purpose of this analysis, the significance of predicting loan risk, and how the model can assist in loan approvals.
- **Results**: Present the results in a bulleted list:
  - Accuracy score
  - Precision score for both healthy and high-risk loans
  - Recall score for both healthy and high-risk loans
- **Summary**: 
  - Summarize the model's performance.
  - Provide a recommendation on whether the model should be used for loan approval purposes. Justify the recommendation based on the evaluation results.

## Files in this Repository

- **lending_data.csv**: The dataset containing historical lending information.
- **starter_code.ipynb**: A Jupyter notebook containing starter code for loading data, training the model, and performing evaluation.
- **README.md**: This file, which includes an overview of the challenge and instructions for running the code.

## Requirements

To run this challenge, the following dependencies need to be installed:

- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

These can be installed using pip:

```bash
pip install pandas scikit-learn matplotlib seaborn
