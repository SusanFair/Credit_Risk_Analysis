# Credit_Risk_Analysis

## Overview of the analysis: 
In this analysis activity we are using several sampling mothods to train and deliverer the most effective model. This analysis will include:
* Oversampling with RandomOverSampler & SMOTE algorithms,
* Undersampling using the ClusterCentroids algorithm,
* Combination of over and undersampling with SMOTEENN algorithm, and 
* 2 machine learning models BalancedRandomForestClassifier and EasyEnsembleClassifier

The comparison of the 2 models used to reduce bias were then used to predict credit risk. 

This report will provide the analysis of the performance of the models and a recommendation of which, if any should be used in predicting credit risk.


## Results: 
The results of the analysis were as follows.  We are looking at balanced accuracy scores, precision and recall scores as our method of comparison


## Over Sampling:<br>
#### Random Oversampling<br>
* balanced accuracy score: .617
* precision: avg .99
* recall score: avg .60

![Random Oversampling](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/random_oversampling.PNG)


#### SMOTE Oversampling<br>
* balanced accuracy score: .662
* precision: avg .99
* recall score: avg .69

![SMOTE](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/SMOTE.PNG)

## Under Sampling:<br>
#### Under Sampling with ClusterCentroids<br>
* balanced accuracy score: .545
* precision: avg .99
* recall score: avg .40

![ClusterCentroids](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/under_sampling_ClusterCentroids.PNG)


## Combination (Over and Under) Sampling 
#### SMOTEENN<br>
* balanced accuracy score: .677
* precision: avg .99
* recall score: avg .58

![SMOOTEENN](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/smooteenn.PNG)

## Ensemble Learners: <br>
#### Balanced Random Forest Classifier
* balanced accuracy score: .683
* precision: avg 1.00
* recall score: avg 1.00

![Balanced Random Forest](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/balanced_random_forest_imbalanced.PNG)


#### Easy Ensemble AdaBoost Classifier<br>
* balanced accuracy score: .932
* precision: avg .99
* recall score: avg .94

![Adaboost](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/Resources/easy_ensemble_adaboost.PNG)<br>


#### Analysis Notebooks: Analysis performed can be found in the 
* [Credit Risk Resampling Notebook](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)
* [Credit Risk Ensemble Notebook](https://github.com/SusanFair/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)



## Summary: 
In summary the overall precision numbers of all 6 methods were good although some of the precision scores for high risk loans were quite low.  Recall scores varied across methods with SMOTE and Random Forest being the lowest. 

The Combindation (Over and Under) Sampling with SMOTEENN results were comparible with the others on precision however recall on high risk was .77 and low_risk was .58.  Good numbers especially on the high risk decisions.

The models really excelled however with the ensemble learning.  Radom Forest came in with precision numbers of .88 for high risk and 1.00 for low risk.  Putting it near the top.  Recall numbers were lower however with .37 high risk and 1.00 for low risk.  This showed a weakness on the high risk decisions.

#### Recommendation
The best overall scores were with the Easy Ensemble AdaBoost Classifier and this method would be the recommended model to use.

While the precision for high risk was a low .09 vs low risk of 1.00 this was offset by the recall numbers which were .92 for high risk and .94 for low risk.  This would indicate that the proportion of actual positives that were identified correctly was very high for high risk lowas.  Since these high risk loans would endanger the stability of the banking system this would be a key identifier in making a model selection.   And with a balanced accuracy score of .931 it also shows it's value.
