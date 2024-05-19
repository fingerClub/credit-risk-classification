# credit-risk-classification

help with programming from tutoring services.

# Module 10 Report 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of the analysis is to assess the efficacy of the created model in predicting whether a borrower will default on their loan. The data gave the size of loan the borrower had asked for, the interest rate of the loan, their income, their amount of debt to their income as a percentage, the number of accounts they have, the ammont of derogatory marks on their credit score, and the total ammount of debt they have. The model needed to predict whether the borrower was at high-risk or not of defaulting on their loan. The dataset had a sample size of 77535 borrowers.

All in the CSV were marked as features while loan status was marked as a label. These were divded into two dataframes with X = features and y = the loan status label. The datasets were split into training and testing data, using the training data to train the data set to predict loan status, and the test data to test efficacy of the created model. a LogisticRegression model was created and fit with training data. The model was then used to predict loan risk on test data and a confusion matrix was generated and then a classification report.

Describe the stages of the machine learning process you went through as part of this analysis.
Briefly touch on any methods you used (e.g., LogisticRegression, or any other algorithms).
Results

## accuracy scores and the precision and recall scores
* Accuracy
  Accuracy for the model is .99 which indicatees that 99% of total predictions are correct. F-1 score for class 0 is a 1 meaning it has an excellent balance of precesion and recall. the F-1 score for class 1 is .89 which indicates it is weaker in precision and recall for predicting those at risk for loans.
* Precision
  1. Class 0 has pristine precision (1), meaning there are no false positives in determining a healthy loan, all selected as a healthy loan are healthy loans
  2. Class 1 has a precision of .84 meaning it occasionally will classify a borrower with a healthy loan as one at high risk. 
* Recall
  1. Class 0 is near pristine (.99), meaning there are little to no false negatives in determining a healthy loan, meaning almost all who are identified as high risk are likely to be high risk.
  2. Class 1 is .94, meaning it occasionally will not identify an at-risk borrower as being an at-risk borrower.


## Conclusion
In determining those who will have a healthy loan, the model is almost spot-on, as indicated by its f-1 score of 1. Because this class is so effective, relying on the model to predict class zero values will almost always predict healthy loan borrowers. Healthy loan borrowers are those who are credit-worthy and are best customers to offer services to. Overall, there are far less borrowers at risk of defaulting on their loan. such a small sample size likely explains why the model is less accurate in predicting those who are at risk. If it's financially best to only offer services to low-risk borrowers, then it is recommended that the model is used to identify those with healthy loans (class 0) to minimize risk to the company due to its f-1 score, recall, and precision for those with healthy loans. With an accuracy of .99, this is a great base model for predicting borrower creditworthiness.
