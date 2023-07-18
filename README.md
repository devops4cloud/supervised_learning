Supervised Machine Learning - Loan Analysis

## Overview of the Analysis

Supervized learning is machine learning algorithm which makes estimates and predictions by learning and emulating data that was fed to the system in the form of training data.

Credit worthiness of an individual can be based on different factors like income, currently outstanding debt amount, debt to income ratio, previously derogatory remarks, etc. 
Overall, all these different variables and chances of a person defaulting on their payments.

In this, program we attempt to create a supervized learning where we use different variables to assess the healthiness of the loan. We also explore confusion matrix and classification metrics to check the efficiency of the model that we made.

### Purpose
The program uses historic set of data available about the borrowers and loan status. Based on this data, the machine learning algorithm is used to train and test the acccuracy and precision of the predictions. The model splits the data into training and testing sets.

### Data Used for the Analysis
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
 * Accuracy Score <br>
    <img title="Imbalanced Accuracy Score" alt="Alt text" src="/images/imbalanced_accuracy.png"> <br>
 * Confusion Matrix  <br>
    <img title="Confusion Matrix" alt="Alt text" src="/images/imbalanced_confusion.png"> <br>
 * Classification Report  <br>
    <img title="Classfification Report" alt="Alt text" src="/images/imbalanced_classification.png"> <br>

* Machine Learning Model 2: Logistic Regression with balanced data 
 * Accuracy Score <br>
    <img title="Accuracy Score" alt="Alt text" src="/images/balanced_accuracy.png"> <br>
 * Confusion Matrix  <br>
    <img title="Confusion Matrix" alt="Alt text" src="/images/balanced_confusionmatrix.png"> <br>
 * Classification Report  <br>
    <img title="Classfification Report" alt="Alt text" src="/images/balanced_classification.png"> <br>


## Summary

The models evaluated provide a good accurate possibilities of predicting future loan health. It was important to re-balance the data to get this level of accuracy and precision in predicting the outcome of the loans. In conclusion, the re-balanced model seems to be a better predictor of the healthiness of a loan.
