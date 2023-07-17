# Credit-Risk-Classification (Supervised Machine Learning Model)

Overview of the Analysis

The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.
I split the data into training and testing sets and created a logistic regression model with the original data.



Results
Logistic Regression Model 1:
Precision: The logistic regression model predicts a healthy, low-risk loan with 100% precision. It predicts a high-risk loan with lower precision at 87%. The balanced accuracy of the model is 94%.

             precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384

Accuracy: 99%
Recall: 94% 


Logistic Regression Model 2:
Precision: The logistic regression model predicts a healthy, low-risk loan with 100% precision. It predicts a high-risk loan with lower precision at 87%. The balanced accuracy of the model is 100%.

            precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      1.00      0.93       625

    accuracy                           1.00     19384
   macro avg       0.94      1.00      0.96     19384
weighted avg       1.00      1.00      1.00     19384

Accuracy: 100%
Recall: 100%


The goal is to recommend that a loan company utilizes the model that minimizes the number of false positives and negatives. You specifically want to focus on the false negatives, because that ultimately would cost the company more money. 

With incorrect predictions we have two issues. 
1. false positives (where users are flagged as risky, but are actually healthy)
2. false negatives (where users are not flagged as risky but are actually risky)
   both cases have its costs. It is important to predict both 1s and 0s. Therefore, model should have good accuracy in terms of both.
