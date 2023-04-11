# Credit_Risk_Analysis

## Overview of the analysis: 
In this analysis activity we are using several sampling mothods to train train and deliverer the most effective model. This analysis will include:
* Oversampling with RandomOverSampler & SMOTE algorithms,
* Undersampling using the ClusterCentroids algorithm,
* Combination of over- and undersampling with SMOTEENN algorithm, and 
* Compare 2 machine learning models BalancedRandomForestClassifier and EasyEnsembleClassifier

The comparison of the 2 models used to reduce bias were then used to predict credit risk. 

This report will provide the analysis of the performance of the models and a recommendation of which, if any should be used in predicting credit risk.


## Results: 
The results of the analysis were as follows.  We are looking at balanced accuracy scores, precision and recall scores as our method of comparison


## Over Sampling:<br>
#### Random Sampling<br>
* balanced accuracy score
* precision
* recall score
<br>
![Alt text](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/random_sampling.PNG)


#### SMOTE<br>
* balanced accuracy score
* precision
* recall score
<br>
![Alt text](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/SMOTE.PNG)

## Under Sampling:<br>
#### Under Sampling with ClusterCentroids<br>
* balanced accuracy score
* precision
* recall score
<br>
![ClusterCentroids](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/under_sampling_ClusterCentroids.PNG)


## Combination (Over and Under) Sampling 
#### SMOTEENN<br>
* balanced accuracy score
* precision
* recall score
<br>
![SMOOTEENN](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/smooteenn.PNG)

## Ensemble Learners: <br>
#### Balanced Random Forest Classifier
* balanced accuracy score
* precision
* recall score
<br>
![Balanced Random Forest](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/balanced_random_forest_imbalanced.PNG)


#### Easy Ensemble Classifier<br>
* balanced accuracy score
* precision
* recall score
<br>
![Adaboost](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/easy_ensemble_adaboost.PNG)<br>

#### Analysis Notebooks: Analysis performed can be found in the 
* [Credit Risk Resampling Notebook](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)
* [Credit Risk Ensemble Notebook](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)



## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning. There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)

 Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)