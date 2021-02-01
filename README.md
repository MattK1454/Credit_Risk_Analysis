# Credit Risk Analysis

## Overview

The purpose of this analysis is to analyze data regarding loan applications to explore which of six machine learning models 
will best predict a loan applicant as being high or low risk for a loan.

## Results

It will be of benefit to outline some of the terms used to evaluate these models prior to the start of the analysis.
 - Balanced accuracy score: A measure of how well the trained model did in predicitin classification outcomes already provided in the dataset. The higher the score
 the better the model at using the input features to classify the outcomes.
 - classification report:
 	- The "pre" stands for precision of the model in regards to the possible outcome (classifying a loan applicant as 'high_risk' or 'low_risk'). This is
	how often the prediction is actually true.
	- "rec" stands for recall or sensitivity of the test to determine possible outcome. This is how often the model accurately determined the true status
	of a applicant.
	- f1 score is measure of the model's balance between precision and recall.
 - In the top half of every scoring snapshot, there is a confusion matrix present to provided the raw values for: 
 	- True positve (top-left)
	- False Negative (top-right)
	- False Positive (bottom-left)
	- True Negative (bottom-right)

- Naive Oversampling

![Navie Oversampling balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/naive_over_sampling_balanced_score.png)

Here the balanced accuracy score of the Naive Oversampling is: 67.70%.

![Naive Oversampling matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/naive_over_sampling_matix_scores.png)

The scores for the Naive Oversampling method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 76%; low_risk = 59%
	- f1: high_risk = 2%; low_risk = 76%
	
In the Naive Oversampling model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. In the Naive Oversampling model, the precision of determining the 'low_risk' 
applicants is 100%. The sensitivity to picking up a 'low_risk' applicant is 59%. The f1 for 'low_risk' applicants is 76%.

- SMOTE

![SMOTE balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTE_balanced_score.png)

The balanced accuracy score of the SMOTE algorithm is: 66.24%

![SMOTE matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTE_matrix_scores.png)

The scores for the SMOTE method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 63%; low_risk = 69%
	- f1: high_risk = 2%; low_risk = 82%
	
In the SMOTE model, the precision of determining the 'high_risk' applicants is only 1%. The sensitivity to picking up a 
'high_risk' applicant is 63%. The f1 for high_risk applicants is 2%. In the SMOTE model, the precision of determining the 'low_risk' 
applicants is 100%. The sensitivity to picking up a 'low_risk' applicant is 69%. The f1 for 'low_risk' applicants is 82%.

- Cluster Centroids

![Cluster Centroids balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/clustercentroids_under_sampling_balanced_score.png)

The balanced accuracy score of the Cluster Centroids algorithm is: 54.42%

![Cluster Centroids matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/clustercentroids_under_sampling_matrix_scores.png)

The scores for the Cluster Centroids method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 76%; low_risk = 42%
	- f1: high_risk = 1%; low_risk = 59%
	
In the Cluster Centroids model, the precision of determining the 'high_risk' applicants is only 1%. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 1%. In the Cluster Centroids model, the precision of determining the 'low_risk' 
applicants is 100%. The sensitivity to picking up a 'low_risk' applicant is 42%. The f1 for 'low_risk' applicants is 59%. 

- SMOTEEN

![SMOTEEN balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEENN_balanced_score.png)

The balanced accuracy score of the SMOTEEN algorithm is: 64.89%

![SMOTEEN matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEENN_matrix_scores.png)

The scores for the SMOTEEN method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 70%; low_risk = 59%
	- f1: high_risk = 2%; low_risk = 75%
	
In the SMOTEEEN model, the precision of determining the 'high_risk' applicants is only 1%. The sensitivity to picking up a 
'high_risk' applicant is 70%. The f1 for high_risk applicants is 2%. In the SMOTEEN model, the precision of determining the 'low_risk' 
applicants is 100%. The sensitivity to picking up a 'low_risk' applicant is 59%. The f1 for 'low_risk' applicants is 75%.

- Balanced Random Forest Classifier

![Balanced Random Forest Classifier balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/balanced_random_forest_balanced_score.png)

The balanced accuracy score of the Balanced Random Forest Classifier algorithm is: 78.85%

![Balanced Random Forest Classifier matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/balanced_random_forest_matrix_scores.png)

The scores for the Balanced Random Forest Classifier method are:
	
	- pre: high_risk = 3%; low_risk = 100%
	- rec: high_risk = 70%; low_risk = 87%
	- f1: high_risk = 6%; low_risk = 93%
	
In the Balanced Random Forest Classifier model, the precision of determining the 'high_risk' applicants is 3%. The sensitivity to picking up a 
'high_risk' applicant is 70%. The f1 for high_risk applicants is 6%. In the Balanced Random Forest Classifier model, the precision of determining the 'low_risk' 
applicants is 100%. The sensitivity to picking up a 'low_risk' applicant is 87%. The f1 for 'low_risk' applicants is 93%. 

- Easy Ensemble Classifier

![Easy Ensemble Classifier balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/easy_ensemble_balanced_score.png)

The balanced accuracy score of the Easy Ensemble Classifier algorithm is: 93.17%

![Easy Ensemble Classifier matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/easy_ensemble_matrix_scores.png)

The scores for the Easy Ensemble Classifier method are:

- pre: high_risk = 9%; low_risk = 100%
- rec: high_risk = 92%; low_risk = 94%
- f1: high_risk = 16%; low_risk = 97%
	
In the Easy Ensemble Classifier model, the precision of determining the 'high_risk' applicants is 9%. The sensitivity to picking up a 
'high_risk' applicant is 92%. The f1 for high_risk applicants is 16%. In the Easy Ensemble Classifier model, the precision of determining the 'low_risk' 
applicants is 100%. The sensitivity to picking up a 'low_risk' applicant is 94%. The f1 for 'low_risk' applicants is 97%.

## Summary

Reviewing results of the various models, it can be noted that a combinatorial approach to sampling the data is best for the class oversized dataset. The best
scores from the machine learning models used here belong to the Easy Ensemble Classifier model. It possesses the best scores for precision and sensitivity 
and the balance of the two out of all the models. The Easy Ensemble Classifier also possesses the highest balanced accuracy score detailing how often the
prediction was correct when measured against the known answer. 

Recommendation: It is my recommendation the Easy Ensemble Classifier model be utilized to assess loan applicant credit risk status.