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
*Machine Learning Model 2: Logistic Regression Model based on the Resampled Data (oversampled data refers to a dataset that has been artificially modified to address class imbalance. Class imbalance occurs when one class has significantly fewer samples than the other class(es) in a binary or multi-class classification problem. In such cases, the model may have difficulty learning patterns from the minority class due to the unequal distribution of samples).

Below, the results of both models.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  *Accuracy: 99%
  *Precision for 0 (Low-Risk Loan): 100%
  *Precision for 1 (High-Risk Loan): 85%
  *Recall for 0 (Low-Risk Loan): 99%
  *Recall for 1 (High-Risk Loan): 91%%

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
