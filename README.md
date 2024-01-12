# credit-risk-classification

In this challenge I used machine learning techniques to analyze a dataset which contained lending practices of a lending services company so that a model can be built to determine borrowers' creditworthiness. 

The analysis considered factors such as:
- the size of the loan
- interest rate
- ratio of debt to income
- income
- accounts held by borrower
- total debt 
- points against the borrower

The data was split into training and testing sets, where the training set was used for the logistic regression model using the LogisticRegression module from scikit-learn and the second used the RandomOverSampler module from imbalanced-learn. 

# Results
The LR model using the LogisticRegression module:
- Precision: 100[0] & 85[1]
- Accuracy Score: 0.9520479254722232
- Recall: 99%[0] & 91%[1]
The balanced accuracy score is 95%. According to the LR model, there is 100% precision when predicting a healthy low-risk loan and 85% precision when predicting high-risk loans. The model predicts healthy loans more precisely than high-risk loans. 

The LR model using the RandomOverSampler module:
- Precision: 100%[0] & 84%[1]
- Accuracy Score: 0.9936781215845847
- Recall: 99%[0] & 99%[1]
The balanced accuracy score is 99%. The resampled LR model predicts healthy, low-risk loans with 100% precision and predicts high-risk loans with a precision of 84%. This model does a better job that the other model as it catches more mistakes with the labelling of loans as high or low-risk. 

# Summary 
The LR model using the RandomOverSampler has a higher accuracy rate so it's less likely to predict a false negative result but it according to the confusion matrix is likely to predict more false-positives than the other model. I'd recommed this model to the company as the model has a higher accuracy score and predicts fewer false negatives. 