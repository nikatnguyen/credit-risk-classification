# Module 12 Report Template

## Overview of the Analysis

 This analysis is meant to determine the creditworthiness of borrowers based on loan risk data from a peer-to-peer lending services company. This model was designed to predict high-risk versus healthy loans. 

The variables I was trying to predict was the loan_status, which were already encoded into a binary classification of 0 (meaning healthy loan) and 1 (being high-risk). 

 My process involved basic training and fitting.After loading the data, I separated the data into labels and features, with labels as the "loan_status" column and features being the rest. I then split the data into training and testing datasets using the train_test_split module from sklearn.model_selection. Once they were split, I proceeded to create my logistic regression model using the training data, and I saved predictions on the testing data labels using model.predict. Finally, I generated a confusion matrix for my model and printed a classification report. 


## Results

* Machine Learning Model 1: Predicting 0 (healthy loans)
  * Model 1 Accuracy score (macro): 0.92 
   * The model is 92% accurate
  * Precision: 1.00 
   * 100% of the class was found over the whole class
  * Recall: 0.99 -> 99% of the class was correctly classified
   * 99% of the class was correctly classified


* Machine Learning Model 2: Predicted 1 (high-risk loans)
  * Model 2 Accuracy (macro): 0.95 
   * The model is 95% accurate
  * Precision: 0.85
   * 85% of the class was found over the whole class
  * Recall: 0.91 
   * 91% of the identified class was correctly classified
  
  
## Summary
The model that seems the best to use would be the first model, which predicted healthy loans. While its macro accuracy score (0.92) was lower than the high-risk accuracy score (0.95), it scored higher for its precision and recall scores, correctly finding and identifying a large majority of healthy loans. 
For the purpose of trying to identify high-risk loans, neither model would be sufficient to use. The first model predicting healthy loans would be futile to use, and the second model predicting high-risk loans is mostly accurate but requires more work to ensure that it more accurately predicts high-risk loans. 
