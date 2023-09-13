# Credit-risk-classification-
Overview of the Analysis

The purpose of this analysis is to to assess and improve the performance of a machine learning model for predicting loan risk. The data had financial 
information of borrowers on loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and loan status.
The goal of the analysis is to predict the "Loan Status" or the outcome of the loan application. A value of 0 in the “loan_status” column means that the loan is healthy and a value of 1 means that the loan has a high risk of defaulting. Based on analysis 75,036 loans are in category 0 and 2,500 are in category 1.


After initial exploration of the dataset to understand its structure, the target variable "Loan Status" was identified and relevant features were 
selected for the machine learning model. The dataset was split into training and testing sets to evaluate the model's performance. "Logistic Regression 
model"  and "Logistic regression with data resampling" was selected for this problem and was fit to the training data. Resampling was done to 
address class imbalance which include oversampling the minority class (56271 samples in both category 0 and 1). Finally, predictions were then made on 
the testing data. The model was then evaluated using confusin matrix and classification report. 


Results

Model 1 Logistic Regression:
Accuracy: 0.992, Precision score for 0: 1.00, Precision score for 1:0.85, Recall score for 0:0.99, Recall score for 1:0.91

Model 2 Logistic Regression with data resampling:
Accuracy: 0.993, Precision score for 0: 1.00, Precision score for 1:0.84, Recall score for 0:0.99, Recall score for 1:0.99

Summary

Model 2 improves the recall score for class 1 which means it is much better at capturing high-risk loans and Model 2 also has a higher F1-score 
for class 1 which shows a better balance between precision and recall for identifying high-risk loans. Therefore, based on the provided metrics 
and the context of loan risk assessment, Model 2 is likely the better-performing model. In a loan risk assessment, correctly identifying high-risk 
loans (class 1) might be more important to minimize financial losses.




