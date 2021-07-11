# Credit Risk Analysis


## Overview:


The purpose of this analysis was to use machine learning algorithms to predict credit risk.  The dataset analyzed was a compilation of credit card credit information from LendingClub.  Six different machine learning algorithms were used on the dataset to compare credit risk predictions and determine which model predicted credit risk the best.  Because the dataset was unbalanced with more low-risk than high-risk datapoints, the libraries from imbalanced-learn and scikit-learn were used in this analysis. Two oversampling models, RandomOverSampler and Smote, one undersampling method, Cluster Centroid, one combination method, SMOTEENN, and two ensemble learners, Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier were used to predict credit risk on the LendingClub dataset.  All of the analyses were performed in Jupyter Notebook.


## Results:


### Oversampling 


#### RandomOverSampler


![randomoversampler](https://user-images.githubusercontent.com/78699521/125178028-b6e88300-e195-11eb-8d00-a7d96178bcde.png)


* balanced accuracy score: 0.6870039085293


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low-risk: 1.00


* recall score:
    * avg: 0.60
    * high-risk: 0.77
    * low-risk: 0.60


#### SMOTE


![smote](https://user-images.githubusercontent.com/78699521/125178034-c36cdb80-e195-11eb-9a04-49f347462079.png)

* balanced accuracy score: 0.6625110564143412


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low-risk: 1.00


* recall score:
    * avg: 0.69
    * high-risk: 0.73
    * low-risk: 0.69


### Undersampling


#### Cluster Centroids


![clustercentroids](https://user-images.githubusercontent.com/78699521/125178036-c962bc80-e195-11eb-8aa3-1f5ca12a32ad.png)

* balanced accuracy score: 0.5442661782548694


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low-risk: 1.00


* recall score:
    * avg: 0.40
    * high-risk: 0.69
    * low-risk: 0.40


### Combination Sampling


#### SMOTEENN


![smoteenn](https://user-images.githubusercontent.com/78699521/125178039-cf589d80-e195-11eb-8602-a1ce04a01376.png)

* balanced accuracy score: 0.6400726134353378


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low-risk: 1.00


* recall score:
    * avg: 0.58
    * high-risk: 0.70
    * low-risk: 0.58


### Ensemble Learners


#### Balanced Random Forest Classifier


![brfc](https://user-images.githubusercontent.com/78699521/125178042-d67fab80-e195-11eb-95d8-6ee6eb5d7ecc.png)

* balanced accuracy score: 0.7885466545953005


* precision score: 
    * avg: 0.99
    * high-risk: 0.03
    * low-risk: 0.99


* recall score:
    * avg: 0.87
    * high-risk: 0.70
    * low-risk: 0.87


#### Easy Ensemble AdaBoost Classifier


![eec](https://user-images.githubusercontent.com/78699521/125178044-daabc900-e195-11eb-8112-695e3884dfce.png)

* balanced accuracy score: 0.9316600714093861


* precision score: 
    * avg: 0.99
    * high-risk: 0.09
    * low-risk: 1.00


* recall score:
    * avg: 0.94
    * high-risk: 0.92
    * low-risk: 0.94


## Summary:

The balanced accuracy score, or percentage of correct credit predictions ranged from 0.54(54% correct) to 0.93(93% correct) among the tested models, with the undersampling technique, Cluster Centroids, doing the worst, and the ensemble learner, Easy Ensemble AdaBoost Classifier, receiving the highest score.  The precision scores of all models were in a similar range, with all models having an average score of 0.99.  The average is misleading as the precision for high-risk credit was between 0.01 and 0.09 for all models, while the precision for low-risk credit was much higher varying from 0.99 to 1.00 for all models.  Looking at precision, the Easy Ensemble AdaBoost Classifier algorithm had better precision for high-risk credit with a score of 0.09, indicating a 9% reliability of a correct classification for high risk credit.  Recall scores varied a lot more between the tested algorithms, with average scores ranging from 0.40 to 0.94.  Different from the precision scores, recall scores tended to be higher for high-risk credit than low-risk credit, indicating all models had more sensitivity to correctly predict high credit risk.  The undersampling model, Cluster Centroids, had the lowest recall score overall with an average score of 0.40.  Both ensemble learners had higher recall and high-risk precision scores than the other algorithms tested, with the Easy Ensemble AdaBoost Classifier receiving the best scores overall.  Of the six models tested the Easy Ensemble AdaBoost Classifier appears to be the best at predicting high risk credit, with a balanced accuracy score of 0.93, the highest high-risk precision score at 0.09, and the greatest recall scores at 0.92 for high-risk and 0.94 for low-risk credit.  This model has a lot of sensitivity to detect high risk credit but will also have a lot of false high risk predictions because of its low high-risk precision score of 0.09.  This means many consumers applying for credit cards from LendingClub may be unfairly rejected by being falsely categorized as high-risk.  A different model with higher precision and a decent recall score would be preferable for those seeking credit. 
