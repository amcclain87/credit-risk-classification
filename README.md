# credit-risk-classification
Module 20 Challenge


## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
  * The purpose of the analyis is to determine the level of risk present for people applying for loans. It looks at the characteristics present for people with healthy and unhealthy loans.

* Explain what financial information the data was on, and what you needed to predict.
  * The data that was included in the analysis for the each applicant was loan size, the interest rate of the loan, the applicant's income, a dept to income ration, the number of accounts held by the applicant, whether they have any marks against their credit, and the amount of debt they currently have.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
  * balance: the amount of people healthy or unhealthy loans
  * distinct_values: the ammount of people with health or unhealthy loans within the resampling data

* Describe the stages of the machine learning process you went through as part of this analysis.
  1) seperate the target variable(loan status) and assign it to the y variable. The rest of the variables are assigned to X
  2) the X and y variables are then randomly split into training and test variables
  3) a logistic regression model was created and then fit to the training data, which then allowed for predictions to be made about loan status using the test data from the X variable
  4) these steps were recreated using resampled training data.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
  * The method used is logistic regression, which is a statistical method that allows for predictions of an outcome. In this case, whether a loan will be healthy or unhealthy. 
The second method used resampling, which increased the sample data for the unhealthy loans from 2500 to 75036, which allowed for a greater ability to train this model for more accurate predictions.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
     * Accuracy: 95.2%
     * Precision: 100% of the predictions for healthy loans were caught, 85% of unhealthy loans were caught
     * Recall: 99% of healthy loans were identified, and 91% of unhealthy loans were idenitified


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
     * Accuracy: 99.4%
     * Precision: 100% of the predictions for healthy loans were caught, 84% of unhealthy loans were caught
     * Recall: 99% of healthy loans were identified, and 99% of unhealthy loans were idenitified
    
    
    
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
  * Model 2 had a higher recall for unhealthy loans and a higher overall accuracy rate of 99.4%

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  * From a finacial standpoint, it would be more important to be able to identify the unhealthy loans to try to reduce risk when approving loans.

If you do not recommend any of the models, please justify your reasoning.
  *Both methods appear to yield results with high accuracy results.
