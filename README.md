Correctly predicted false positives with a 79% percision by applying XGboost ensemble boosting classification.   

# Analysis

**Data:**  from 1994 census.
*consists of 32k observations and 15 features.* 

**Problem:** The task is to accurately predict if a person has an income greater than 50k or less than 50k. 

We're given 15 features per person; using these features the model will predict an income as being greater than 50k or less than 50k. 

* more than 50k is mapped to 1. 
* less than 50k is mapped to 0.
* true positive: income > 50k or 1 mapping
* true negative: income < = 50k or 0 mapping

*false positive* = prediction of income greater than 50k when its true value is less than 50k.

In this instance we want to reduce the number of false positives. Therefore, we use precision as our metric judging the accuracy of our trained ML model.

Model Percision Scores: 
1. XGboost (Ensemble Boosting Classifer): 0.794
1. Support Vector Machine: 0.740
1. Logistic Regression: 0.731
1. Multilayer Perceptron NN Classifier: 0.610

XGboost appears to be the best model here.

This Dataset was obtained from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/census+income)
