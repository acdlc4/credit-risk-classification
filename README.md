# credit-risk-classification - Module 20 Report


## Overview of the Analysis

* Purpose: Build of a loan risk model to be trained and evaluated using various techniques

* Data source: Historical lending activity from a peer-to-peer lending services company to predict creditworthiness of borrowers

* Variables: 'loan_status' is the variable being predicted by the model being built, which indicates whether or not the loan is considered 'healthy' (i.e. '0' value) or high-risk (i.e. '1' value)
* Procedures taken:
    1) Data wrangling using pandas, including separation of the variable to be tested and the remainder of the data
    2) Create separate training and testing datasets using scikit-learn's 'train_test_split' function
    3) Create a logistic regression model using scikit-learn's 'LogisticRegression' function and 'predict' function to test the variable
    4) Evaluate the model performance with scikit-learn's 'classification_report' function and summarize the report

## Results

![Classification Results](https://github.com/acdlc4/credit-risk-classification/blob/main/Resources/class_report.png)

* Machine Learning Model Results:
    * Very strong results shown, as all figures below are above 0.90:
        
        1) Accuracy:  0.99
        2) Precision: 0.92 (macro average)
        3) Recall:    0.97 (macro average)

## Summary

After review of the classification report of the model results, the recommendation is to use the model as built as all three results (i.e. accuracy, precision, and recall) of the model are above 0.90, indicating very strong results.  Consideration for further review for outlier cases for high-risk loans may be needed to further minimize lending risk to the company.
