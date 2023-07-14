# Module 12 Report Template

## Overview of the Analysis

This analysis aims to determine borrowers' creditworthiness from a dataset of historical lending activity from a peer-to-peer lending services company. The following data fields were given:

* Loan Amount
* Interest Rate
* Borrower Income
* Debt to Income Ratio
* Number of Accounts
* Derogatory Marks on Credit Report
* Total Debt
* Loan Status
* Note: all the above data fields are regarding the borrower

The variables that were predicted are:
*0 for Low-Risk Loan
*1 for High-Risk Loan

First, the data needs to be split into 2:
*Loan Status
*Loan Amount, Interest Rate, Borrower Income, Debt to Income Ratio, Number of Accounts, Derogatory Marks on Credit Report and Total Debt

Once the split happens, a count of the variable is performed. The results for the variables are:
*0 for Low-Risk Loan: 75036
*1 for High-Risk Loan: 2500

Then. There are 2 Logistic Regression Models that are used with the following data:
*Machine Learning Model 1: Logistic Regression Model based on the Original Data (the data provided by the peer-to-peer lending services company).
*Machine Learning Model 2: Logistic Regression Model based on the Resampled Data (oversampled data refers to a dataset artificially modified to address class imbalance. Class imbalance occurs when one class has significantly fewer samples than the other class(es) in a binary or multi-class classification problem. In such cases, the model may have difficulty learning patterns from the minority class due to the unequal distribution of samples).

Below are the results of both models.

## Results


* Machine Learning Model 1:
  * Accuracy: 99%
  * Precision for 0 (Low-Risk Loan): 100%
  * Precision for 1 (High-Risk Loan): 85%
  * Recall for 0 (Low-Risk Loan): 99%
  * Recall for 1 (High-Risk Loan): 91%

* Machine Learning Model 2:
  * Accuracy: 99%
  * Precision for 0 (Low-Risk Loan): 100%
  * Precision for 1 (High-Risk Loan): 84%
  * Recall for 0 (Low-Risk Loan): 99%
  * Recall for 1 (High-Risk Loan): 99%

## Summary

* The accuracy for Machine Learning Model 1 gives 99% accuracy. Now, the precision when predicting High-Risk Loans is 85%. Although it is a good percentage, the model must be adjusted to increase the numbers. Also, it is important to evaluate once the model is adjusted to see if the precision for the Low-Risk Loan gets affected because it is at 100%.
* The accuracy for Machine Learning Model 2, based on the above metrics, the Logistic Regression Model with over sampled data shows better metrics than the first Logistic Regression model. Even though the precision for the High-Risk Loans decreased by 1%, meaning that out of the 619 instances, it predicted correctly almost 613. The Recall metric improved from 0.91 to 0.99 for the High-Risk Loans, indicating that the model now identifies 99% of the High-Risk Loans compared to 91% for the first Logistic Regression Model.
* It is more important to predict the High-Risk Loans than the others.
* It all depends on which metric is more important for each financial institution. If correctly identifying High-Risk Loans (precision) is the priority, then model 1 may be a better choice than model 2 by 1%. But, if capturing as many Hihgh-Risk Loans as possible, model 2 is better with a recall score of 99% compared to 91% of Machine Learning Model 1.


