

# Risky Business - Analysis 

![Credit Risk](Images/credit-risk.jpg)


--- 

___

### Resampling

> 1.Which model had the best balanced accuracy score?
* __Naive Random Oversampling: 0.66__
* SMOTE Oversampling: 0.63
* Undersampling Cluster Centroids: 0.53
* Combination over- and under-sampling SMOTEENN: 0.64

>
> 2.Which model had the best recall score?
* Naive Random Oversampling: __0.63__
    * high_risk: 0.69 
    * low_risk:  0.63 
* SMOTE Oversampling: 0.65 
    * high_risk: 0.61 
    * low_risk:  __0.65__ 
* Undersampling Cluster Centroids: 0.40
    * high_risk: 0.65 
    * low_risk:  0.40
* Combination over- and under-sampling SMOTEENN: 0.58
    * high_risk: __0.70__ 
    * low_risk:  0.58

* _Best Recall Total: Naive Random Oversampling -> 0.63_
* _Best Recall high_risk: SMOTEEN -> 0.70_
* _Best Recall low_risk: SMOTE -> 0.65_

> 3.Which model had the best geometric mean score?
* _Naive Random Oversampling: 0.66_

* SMOTE Oversampling: 0.63

* Undersampling Cluster Centroids: 0.51

* Combination over- and under-sampling SMOTEENN: 0.64

---



#### Ensemble Learning

> Which model had the best balanced accuracy score?
* Random Forest Classifier: 0.68
* __Easy Ensemble Classifier: 0.76__

> Which model had the best recall score?
* Random Forest Classifier: 0.36
    * high_risk: 1.0
    * low_risk:  0.36
* Easy Ensemble Classifier: __0.99__
    * high_risk: 0.51
    * low_risk:  1.0
>
> Which model had the best geometric mean score?
>


> What are the top three features?

---


