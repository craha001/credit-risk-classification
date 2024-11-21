# credit-risk-classification
Module 20 Challenge

## Overview of the Analysis

### Purpose of the Analysis
The goal for this weeks challenge was to develop a machine learning model to predict loan outcomes based on lending data. This prediction would allow the institution to separate high-risk loans and healthy loans making overall better lending decisions.  
Below is a list of X variabls or Features of machine learning model:  

* loan_size: Size of the loan applied for.
* interest_rate: Interest rate of the loan.
* borrower_income: The income of the borrower.
* debt_to_income: Ratio of debt to income.
* num_of_accounts: Number of accounts held by the borrower.
* derogatory_marks: Negative marks on the borrower’s credit report.
* total_debt: Total debt of the borrower.  

Our Y variable was based on loan_status which was binary.  
0 represents a Healthy Loan  
1 represents a High-Risk Loan.  

For this machine learning process I had to scale the X data to normalize the features for the logistic regression model. Logistic regression models are favorable for analyzing binary data. The random state used for training the model was a random state of 1. 

### Results
Machine Learning Logistic Regression Classification Report:  
![image](https://github.com/user-attachments/assets/3c5c1ece-fbea-4e02-b7f3-a642e6690f20)  

* Accuracy Score: Came out to 99% accuracy indicating the model correctly classified 99% of loans as being either healthy or high-risk
* Precision Scores:
    * Healthy Loan(0): 1.00 meaning no false positives for healhty loans showing the models predicted healthy loans were all correct.
    * High-Risk Loan(1): 0.84 showing there was some false positives for high-risk loans meaning not all the predicted high-risk loans were correct.
* Recall Score:
    * Healthy Loan (0): 0.99 score showing almost all healthy loans were correctly identified.
    * High-Risk Loan (1): 0.99 score showing almost all high-risk loans were correctly identified.

### Summary
I would highly recommend this model due to the accuracy alone. Financial institutions rely heavily on providing loans and having a model which can accurately distinguish between a healthy loan and a high-risk loan proves beneficial. However, I do recommend human oversight as there were instances in which healthy loans were being flagged as high-risk loans. Making sure there is some human oversight provides a standard double-checking process to make sure those who should be allowed loans recieve them. Thus, the logistic regression model makes a great fit for financial risk management due to high accuracy and strong recall for both high-risk and healthy loans.
