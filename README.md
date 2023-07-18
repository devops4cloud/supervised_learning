Supervised Machine Learning - Loan Analysis

## Overview of the Analysis

Supervized learning is machine learning algorithm which makes estimates and predictions by learning and emulating data that was fed to the system in the form of training data.

Credit worthiness of an individual can be based on different factors like income, currently outstanding debt amount, debt to income ratio, previously derogatory remarks, etc. 
Overall, all these different variables and chances of a person defaulting on their payments.

In this, program we attempt to create a supervized learning where we use different variables to estimate credit worthiness. We also explore confusion matrix and classification metrics to check the efficiency of the model that we made.

###Purpose
The program uses historic set of data available about the borrowers and loan status. Based on this data, the machine learning algorithm is used to train and test the acccuracy and precision of the predictions. The model splits the data into training and testing sets.

###Data Used for the Analysis
Data availabe for this analaysis is included in the Resources folder (lending_data.csv). Available data features and labels are as follows.
 - Size of the loan in $
 - Interest Rate of the loan
 - Borrowers income
 - Debt to income ratio of the borrower
 - Number of accounts for the borrower
 - Any negative remarks about the borrower
 - Total debt of the borrower
 - Healthiness of the loan (label)

### Data Balancing
- There were close to 77k records of data which can be used for the analysis
- Evaluating the data available, there was an imbalance of data between healthy (75k) and unhealthy loans(2.5k).


### Steps for Analysis

* Imported the data from the CSV
* Seperated the data into labels and features
* Split the data into training and testing
* Analysed the data using Logistic Regression model
* Measured the outcome using the accuracy, confusion matrix and classification report
* Balanced the data using Random Oversampler and re-ran the analysis

## Results

* Machine Learning Model 1: Logistic Regression with imbalanced data
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2: Logistic Regression with balanced data 
  * Description of Model 2 Accuracy, Precision, and Recall scores.


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
