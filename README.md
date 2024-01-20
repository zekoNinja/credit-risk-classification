# credit-risk-classification
Module 20 Challenge
# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis is to build  a model that can detect and predict creditworthiness of borrowers when you they ask for a loan. 
* The financial information used here in the analysis is : ['loan_size', 'interest_rate', 'borrower_income', 'debt_to_income',
       'num_of_accounts', 'derogatory_marks', 'total_debt']. What is being predicted is `loan_status` Explain what financial information the data was on, and what you needed to predict.
* The values I was trying to predict is either `0` (healthy loan) and `1` (high-risk loan) labels
* Stage I went through to build the Machine learning Mode:
  1- Step 1: Read the `lending_data.csv` data from the `Resources` folder into a Pandas DataFrame.
  2- Step 2: Create the labels set (`y`)  from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.
  3- Step 3: Check the balance of the labels variable (`y`) by using the `value_counts` function.
  4- Step 4: Split the data into training and testing datasets by using `train_test_split`.
* Methods I used for my analysis are : `LogisticRegression` and `LogisticRegression` with resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * for 0 (Health loans) results were as following:
    * Balanced Accuracy Score: 0.9442676901753825
    * Confusion Matrix: recall 100%, precision 100%
  * for 1 (high-risk loan) results were as following:
    * Balanced Accuracy Score: 0.9442676901753825
    * Confusion Matrix: Recall 89% , precision 87%



* Machine Learning Model 2:
  * * for 0 (Health loans) results were as following:
    * Balanced Accuracy Score: 0.9442676901753825
    * Confusion Matrix: recall 99%, precision 90%
  * for 1 (high-risk loan) results were as following:
    * Balanced Accuracy Score: 0.9442676901753825
    * Confusion Matrix: Recall 89% , precision 99%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Choosing between Model 1 and Model 2 really going to depend on the goals we are trying to achive,
  * If the goal to predict label 0(healthy loans) accuratly, then precision and recall are critial, and model 1 might be the best choice for class 0
* However, if the goal is to predict class 1(high-risk loan) then precision is important and model 2 has much higher precision for class 1

However, I recommend using model 2, since high-risk loans are more important 
