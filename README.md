## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis is to build a model that can predict the creditworthiness of borrowers based on historical lending activity. By analyzing past lending behavior and the characteristics of borrowers, the goal is to identify patterns.
* The financial data is on loan_size,interest_rate,borrower_income,debt_to_income,num_of_accounts,derogatory_marks,total_debt,loan_status, we are trying to predict loan_status, which would classify the creditworthiness of the borrower.
* The target variable we're predicting is loan_status.
 
* I started by seperating the target variable loan_status from the other variables (loansize, interest_rate, etc.) so then I split it into training and testing sets using train_test_split. Then using lr.model.fit i trained my model  on X_train and y_train. Then I made the predictions using y_test to see how well the model preforms.
* Then I used LogisiticRegression as my model. I used it because its used for binary classification problems.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Accuracy 99% overall so the model correctly classified 99% of the data
    * Class 0 : precision 1.00
                recall : .99
                F1-score = 1.00
    * Class 1 : precision .85
                recall : .91
                F1-score = .88
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* The logistic regression model achieved an overall accuracy of 99%, which indicates that it performs well in classifying both high-risk(Class 1) and good standing loans (Class 0). For class 0 it showed perfect precisison while in class 1 it kind of performed worse.

 * Given the high overall accuracy and strong recall for Class 1 and Class 0, I would recommend using this logistic regression model. It strikes a good balance between precision and recall for predicting loans.
