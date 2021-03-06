# Supervised Machine Learning and Credit Risk 

## Overview of the Analysis
### Purpose
A hypothetical peer to peer lending services company wants to use machine learning to predict credit risk. They need help building and evalutating several ML models, oversampling and undersampling the data, and evaluating the performance of the models to see how well they predict data. Management believes that this will provide a quicker and more reliable loan experience, and lead to a more accurate identification of good candidates for loans.

## Results
### Outputs from All Six Models
- The naive random oversampling algorithm resulted in a balanced accuracy score of 0.64. The precision score was 1.0 for predicting low risk, but extremely low for predicting high risk (0.01). The recall scores were 0.66 and 0.62 for high and low risk, respectively. <br>
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/ros.png' width=700> </kbd> <br>

- The SMOTE algorithm resulted in a balanced accuracy score of 0.65. The precision for predicting high and low risk was the same as the naive random oversampling algorithm. The recall scores were 0.61 and 0.69 for high and low risk, respectively. <br>
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/SMOTE.png' width=700> </kbd> <br>

- The Cluster Centroids algorithm resulted in a resulted in a balanced accuracy score of 0.55. The precision for predicting high and low risk was the same as the previous two algorithms. The recall scores were 0.68 and 0.41 for high and low risk, respectively. <br>
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/cc.png' width=700> </kbd> <br>

- The SMOTEENN algorithm resulted in a resulted in a balanced accuracy score of 0.64. The precision for predicting high and low risk was the same as all the previous algorithms. The recall scores were 0.72 and 0.57 for high and low risk, respectively. <br>
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/smoteenn.png' width=700> </kbd> <br>

- The Balanced Random Forest Classifier resulted in a resulted in a balanced accuracy score of 0.79. The precision score was 1.0 for predicting low risk, but very low for predicting high risk (0.09). The recall scores were 0.92 and 0.94 for high and low risk, respectively. <br>
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/brf.png' width=700> </kbd> <br>

- The Easy Ensemble Classifier resulted in a resulted in a balanced accuracy score of 0.93. The precision and recall scores for predicting high and low risk were the same as the Balanced Random Forest Classifier. <br>
<kbd> <img src='https://github.com/npantfoerder/credit-risk-analysis/blob/master/Images/ee.png' width=700> </kbd> <br>

## Summary
Undersampling the data using the Cluster Centroids algorithm yielded the lowest balanced accuracy score of 0.55. The precision scores for prediciting high risk was low for all six models. The Balanced Random Forest Classifier and the Easy Ensemble Classifier gave the highest recall scores of 0.92 and 0.94 for high and low risk, respectively. I would recommend to use the Easy Ensemble Classsifer because it had the highest balanced accuracy score of 0.93, although the company should be aware of the implications of the precision scores. The precision score of 0.09 means that a high risk classification is not very reliable. 

#### Resources
- Data Sources: LoanStats_2019Q1.csv
- Software: Python 3.7.3, Anaconda 4.8.3, Scikit-learn 0.23.1, Imbalanced-learn 0.7.0
