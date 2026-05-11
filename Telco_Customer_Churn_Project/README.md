# Telco Customer Churn Prediction using PySpark ML

## Project Overview
This project applies Big Data concepts, data analysis, and machine learning techniques on the Telco Customer Churn dataset.

The goal is to predict whether a telecom customer will leave the company or stay.

## Dataset
The dataset used is:

`WA_Fn-UseC_-Telco-Customer-Churn.csv`

## Problem Statement
Telecom companies need to identify customers who are likely to leave the company.

The target column is:

`Churn`

Where:
- Yes = Customer left the company
- No = Customer stayed with the company

## Tools Used
- Google Colab
- PySpark
- Spark DataFrames
- Spark MLlib
- GitHub

## Data Analysis
We applied Spark DataFrame operations such as:
- groupBy
- count
- average aggregation
- filtering
- churn analysis by contract type
- churn analysis by internet service
- churn analysis by payment method

## Handling String Columns
The dataset contains categorical string columns such as:
- gender
- Partner
- Dependents
- InternetService
- Contract
- PaymentMethod

Machine Learning models cannot use string values directly, so we used:
- StringIndexer
- OneHotEncoder

## Machine Learning Model
The model used is:

`Logistic Regression`

We used Logistic Regression because the target column is binary:
- Churn = Yes
- Churn = No

## Model Evaluation
The model was evaluated using:
- Accuracy
- F1 Score
- Precision
- Recall
- AUC
- Confusion Matrix

## How to Run
1. Open the notebook in Google Colab.
2. Upload the dataset CSV file.
3. Run all cells from top to bottom.

## Conclusion
This project demonstrates how PySpark can be used for data analysis and machine learning. The model predicts customer churn based on customer information such as contract type, tenure, monthly charges, payment method, and internet services.
