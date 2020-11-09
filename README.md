# Supervised Machine Learning and Credit Risk 

## Overview of the Analysis
### Purpose
A hypothetical peer to peer lending services company wants to use machine learning to predict credit risk. They need help building and evalutating several ML models, oversampling and undersampling the data, and evaluating the performance of the models to see how well they predict data. Management believes that this will provide a quicker and more reliable loan experience, and lead to a more accurate identification of good candidates for loans.

## Results
### DataFrames from Google Colaboratory
*Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your resutls.*
- The naive random oversampling algorithm resulted in a balanced accuracy score of 0.64. The precision score was 1.0 for predicting low risk, but extremely low for predicting high risk (0.01). The recall scores were 0.66 and 0.62 for high and low risk, respectively. 
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/vine_reviews.png' width=900> </kbd> <br>

- The SMOTE algorithm resulted in a balanced accuracy score of 0.65. The precision for predicting high and low risk was the same as the naive random oversampling algorithm. The recall scores were 0.61 and 0.69 for high and low risk, respectively.
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/vine_reviews.png' width=900> </kbd> <br>

- The Cluster Centroids algorithm resulted in a resulted in a balanced accuracy score of 0.55. The precision for predicting high and low risk was the same as the previous two algorithms. The recall scores were 0.68 and 0.41 for high and low risk, respectively.
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/vine_reviews.png' width=900> </kbd> <br>

- The SMOTEENN algorithm resulted in a resulted in a balanced accuracy score of 0.64. The precision for predicting high and low risk was the same as all the previous algorithms. The recall scores were 0.72 and 0.57 for high and low risk, respectively.
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/vine_reviews.png' width=900> </kbd> <br>

- The Balanced Random Forest Classifier resulted in a resulted in a balanced accuracy score of 0.79. The precision score was 1.0 for predicting low risk, but very low for predicting high risk (0.09). The recall scores were 0.92 and 0.94 for high and low risk, respectively.
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/vine_reviews.png' width=900> </kbd> <br>

- The Easy Ensemble Classifier resulted in a resulted in a balanced accuracy score of 0.93. The precision and recall scores for predicting high and low risk were the same as the Balanced Random Forest Classifier.
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/vine_reviews.png' width=900> </kbd> <br>

## Summary
*Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.*

#### Resources
- Data Sources: LoanStats_2019Q1.csv
- Software: Python 3.7.3, Anaconda 4.8.3, Scikit-learn 0.23.1, Imbalanced-learn 0.7.0
