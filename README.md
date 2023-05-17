# credit-risk-classification

Notebook for this assignment is in this repo as credit_risk_classification.ipynb

## Analysis

The purpose of these models are to predict which loans are high-risk and which are healthy. 

The csv file proviced used a number of categories associated with a borrower. The "loan_status" column was separated from the dataframe as the y value 
as it provided the outcome that we are trying to predict.

The y value described the loan_status as 0 (healthy) or 1 (high-risk). Value_counts shows that there are 75036 healthy loans and 2500 high-risk loans.

The data was split into training and testing datasets by using train_test_split.

An instance of the logistic regression model was instantiated and the training data was fit to the model. Then a prediction was made using the testing data and the model was evaluated (see results).

As well another Logistic Regression model was created with resampled training data. For this the RandomOverSampler module was used. 

An instance of the oversampler model was created and the original training data was fit. 

The y training value now describes the loan status as 56277 healthy loans and 1875 high-risk loans. 

The LogisticRegression classifier and the resampled data was fit to the model and predictions were made based on the resampled data.

In both instances, the models were evaluated using by taking the accuracy score (both showed 99% accuracy) and generating a confusion matrix. 





## Results



* Machine Learning Model 1:
  * Accuracy: 99%
  * Precision: Healthy Loan= 100%, High-risk Loan= 87%
  * Recall: Healthy Loan = 100%, High-risk Loan= 89%



* Machine Learning Model 2:
  * Accuracy: 99%
  * Precision: Healthy Loan= 100%, High-risk Loan= 87%
  * Recall: Healthy Loan = 100%, High-risk Loan= 89%

## Summary

I did not find that resampling the data provided me with any change. Either model provides an accurate prediction. The models predicted the healthy loans and 
high-risk loans within an acceptable range of accuracy. However to better test if another model would improve, we might look at another way than simply resampling the data, which did not provide any better insight. 



Thanks for reading!
