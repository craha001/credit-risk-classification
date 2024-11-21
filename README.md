# credit-risk-classification
Module 20 Challenge

## Overview of the Analysis

### Purpose of the Analysis
The goal for this weeks challenge was to develop a machine learning model to predict loan outcomes based on lending data. This prediction would allow the institution to separate high-risk loans and healthy loans making overall better lending decisions.  
Below is a list of X variabls or Features of machine learning model:  

loan_size: Size of the loan applied for.  
interest_rate: Interest rate of the loan.  
borrower_income: The income of the borrower.  
debt_to_income: Ratio of debt to income.  
num_of_accounts: Number of accounts held by the borrower.  
derogatory_marks: Negative marks on the borrower’s credit report.  
total_debt: Total debt of the borrower.  

Our Y variable was based on loan_status which was binary.  
0 represents a Healthy Loan  
1 represents a High-Risk Loan.  

For this machine learning process I had to scale the X data to normalize the features for of the logistic regression model. Logistic regression models are favorable for analyzing binary data. The random state used for training the model was a random state of 1. 

### Results
Machine Learning Logistic Regression Classification Report:
Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
