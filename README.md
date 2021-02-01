# Credit Risk Analysis

## Overview

The purpose of this analysis is to analyze data regarding loan applications to explore which of six machine learning models 
will best predict a loan applicant as being high or low risk for a loan.

## Results

It will be of benefit to outline some of the terms used to evaluate these models prior to the start of the analysis.
 - Balanced accuracy score: A measure of how well the trained model did in predicitin classification outcomes already provided in the dataset. The higher the score
 the better the model at using the input features to classify the outcomes.
 - classification report:
 	- The "pre" stands for precision of the model in regards to the possible outcome (classifying a loan applicant as 'high_risk' or 'low_risk').
	- "rec" stands for recall or sensitivity of the test to determine possible outcome.
	- f1 score is measure of the model's balance between precision and recall.
 - In the top half of every scoring snapshot, there is a confusion matrix present to provided the raw values for: 
 	- True positve (top-left)
	- False Negative (top-right)
	- False Positive (bottom-left)
	- True Negative (bottom-right)
	
As this these models were primarily developed with the intention of assessing 'high_risk' applicants, the score in precision, sensitivity, and the balance
between the two will be our primary focus.

- Naive Oversampling

![Navie Oversampling balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/naive_over_sampling_balanced_score.png)

Here the balanced accuracy score of the Naive oversampling is: 67.70%.

![Naive Oversampling matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/naive_over_sampling_matix_scores.png)

The scores for the Naive Oversampling method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 76%; low_risk = 59%
	- f1: high_risk = 2%; low_risk = 76%
	
In the Naive Oversampling model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. This model attempts to deal the oversized aspect of the fact that a majority
of applicants are low_risk. However, since this is the primary model emoployed, it will establish a base line for evaluation.

- SMOTE

![SMOTE balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTE_balanced_score.png)

The balanced accuracy score of the SMOTE algorithm is: 66.24%

![SMOTE matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTE_matrix_scores.png)

The scores for the SMOTE method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 63%; low_risk = 69%
	- f1: high_risk = 2%; low_risk = 82%
	
In the SMOTE model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. 

- Cluster Centroids

![Cluster Centroids balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/clustercentroids_under_sampling_balanced_score.png)

The balanced accuracy score of the SMOTE algorithm is: 54.42%

![Cluster Centroids matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/clustercentroids_under_sampling_matrix_scores.png)

The scores for the Cluster Centroids method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 767%; low_risk = 42%
	- f1: high_risk = 1%; low_risk = 59%
	
In the Cluster Centroids model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. 

- SMOTEEN

![SMOTEEN balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEENN_balanced_score.png)

The balanced accuracy score of the SMOTE algorithm is: 64.89%

![SMOTEEN matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEENN_matrix_scores.png)

The scores for the SMOTEEN method are:
	- pre: high_risk = 1%; low_risk = 100%
	- rec: high_risk = 70%; low_risk = 59%
	- f1: high_risk = 2%; low_risk = 75%
	
In the SMOTEEN model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. 

- Balanced Random Forest Classifier

![Balanced Random Forest Classifier balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/balanced_random_forest_balanced_score.png)

The balanced accuracy score of the SMOTE algorithm is: 78.85%

![Balanced Random Forest Classifier matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/balanced_random_forest_matrix_scores.png)

The scores for the Balanced Random Forest Classifier method are:
	- pre: high_risk = 3%; low_risk = 100%
	- rec: high_risk = 70%; low_risk = 87%
	- f1: high_risk = 6%; low_risk = 93%
	
In the balanced Random Forest Classifier model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. 

- Easy Ensemble Classifier

![Easy Ensemble Classifier balanced accuracy score](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/easy_ensemble_balanced_score.png)

The balanced accuracy score of the SMOTE algorithm is: 93.17%

![Easy Ensemble Classifier matrix scores](https://github.com/MattK1454/Credit_Risk_Analysis/blob/main/Resources/images/easy_ensemble_matrix_scores.png)

The scores for the Easy Ensemble Classifier method are:
	- pre: high_risk = 9%; low_risk = 100%
	- rec: high_risk = 92%; low_risk = 94%
	- f1: high_risk = 16%; low_risk = 97%
	
In the Easy Ensemble Classifier model, the precision of determining the 'high_risk' applicants is only one percent. The sensitivity to picking up a 
'high_risk' applicant is 76%. The f1 for high_risk applicants is 2%. 

## Summary

ABC