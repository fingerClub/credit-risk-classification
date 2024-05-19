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

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1:
Description of Model 1 Accuracy, Precision, and Recall scores.
Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Which one seems to perform best? How do you know it performs best?
Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the 1's, or predict the 0's? )
If you do not recommend any of the models, please justify your reasoning.
