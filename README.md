# Credit Risk Analysis


## Overview:




## Results:


### Oversampling 


#### RandomOverSampler


![randomoversampler](https://user-images.githubusercontent.com/78699521/125178028-b6e88300-e195-11eb-8d00-a7d96178bcde.png)


* balanced accuracy score: 0.6870039085293


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low:risk: 1.00


* recall score:
    * avg: 0.60
    * high-risk: 0.77
    * low:risk: 0.60


#### SMOTE


![smote](https://user-images.githubusercontent.com/78699521/125178034-c36cdb80-e195-11eb-9a04-49f347462079.png)

* balanced accuracy score: 0.6625110564143412


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low:risk: 1.00


* recall score:
    * avg: 0.69
    * high-risk: 0.73
    * low:risk: 0.69


### Undersampling


#### Cluster Centroids


![clustercentroids](https://user-images.githubusercontent.com/78699521/125178036-c962bc80-e195-11eb-8aa3-1f5ca12a32ad.png)

* balanced accuracy score: 0.5442661782548694


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low:risk: 1.00


* recall score:
    * avg: 0.40
    * high-risk: 0.69
    * low:risk: 0.40


### Combination Sampling


#### SMOTEENN


![smoteenn](https://user-images.githubusercontent.com/78699521/125178039-cf589d80-e195-11eb-8602-a1ce04a01376.png)

* balanced accuracy score: 0.6400726134353378


* precision score: 
    * avg: 0.99
    * high-risk: 0.01
    * low:risk: 1.00


* recall score:
    * avg: 0.58
    * high-risk: 0.70
    * low:risk: 0.58


### Ensemble Learners


#### Balanced Random Forest Classifier


![brfc](https://user-images.githubusercontent.com/78699521/125178042-d67fab80-e195-11eb-95d8-6ee6eb5d7ecc.png)

* balanced accuracy score: 0.7885466545953005


* precision score: 
    * avg: 0.99
    * high-risk: 0.03
    * low:risk: 0.99


* recall score:
    * avg: 0.87
    * high-risk: 0.70
    * low:risk: 0.87


#### Easy Ensemble AdaBoost Classifier


![eec](https://user-images.githubusercontent.com/78699521/125178044-daabc900-e195-11eb-8112-695e3884dfce.png)

* balanced accuracy score: 0.9316600714093861


* precision score: 
    * avg: 0.99
    * high-risk: 0.09
    * low:risk: 1.00


* recall score:
    * avg: 0.94
    * high-risk: 0.92
    * low:risk: 0.94


## Summary:

summary and model reccommendation 
