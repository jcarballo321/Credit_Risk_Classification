# Credit_Risk_Classification

## Overview

In this activity I will be using a dataset of historical lending activity froma peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

To achieve this purose I did the following:

* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Predict a Logistic Regression Model with Resampled Training Data

Loans are characterized by either 0 or 1 with 0 signifying that the loan is healthy and 1 signifying that the loan has a high risk of defaulting. 

## Methods Used:

1. Fit a logistic regression model by using the training data (`X_train` and `y_train`).

2. Save the predictions on the testing data labels by using the testing feature data (`X_test`) and the fitted model.

3. Evaluate the model’s performance by doing the following:

    * Calculate the accuracy score of the model.

    * Generate a confusion matrix.

    * Print the classification report.


## Results:

Model 1:


           pre       rec       spe        f1       geo       iba       sup

          0       1.00      1.00      0.89      1.00      0.94      0.90     18755
          1       0.87      0.89      1.00      0.88      0.94      0.88       629

avg / total       0.99      0.99      0.90      0.99      0.94      0.90     19384



Model 2:  

	pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.99      0.99      1.00      0.99      0.99     18765
          1       0.84      0.99      0.99      0.91      0.99      0.99       619

avg / total       0.99      0.99      0.99      0.99      0.99      0.99     19384


## Summary:


The accuracy of Model 1 is highly acceptable since the model categorized the high risk loan with a 94% accuracy.

The accuracy of Model 2 is highly acceptable since the model perfomrmed extremely well with an accuracy of 99%.

In my opinion it is more important to predict the 1's than the zeroes since a loan going into default can be restructured, refincnaced etc. 

In conclusion I would recoomend both Models but I would choose Model 2 over Model 1 due to it beign more accurate.  

