
# hw11-machine-learning 

## Risky Business

![Credit Risk](Images/credit-risk.jpg)


---

## Analysis 

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

In this section, you will train and compare two different ensemble classifiers to predict loan risk and evaluate each model. You will use the [Balanced Random Forest Classifier](https://imbalanced-learn.readthedocs.io/en/stable/generated/imblearn.ensemble.BalancedRandomForestClassifier.html#imblearn-ensemble-balancedrandomforestclassifier) and the [Easy Ensemble Classifier](https://imbalanced-learn.readthedocs.io/en/stable/generated/imblearn.ensemble.EasyEnsembleClassifier.html#imblearn-ensemble-easyensembleclassifier). Refer to the documentation for each of these to read about the models and see examples of the code.

Be sure to complete the following steps for each model:

1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2. Train the model using the quarterly data from LendingClub provided in the `Resource` folder.
3. Calculate the balanced accuracy score from `sklearn.metrics`.
4. Print the confusion matrix from `sklearn.metrics`.
5. Generate a classification report using the `imbalanced_classification_report` from imbalanced learn.
6. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.

Use the above to answer the following:

> Which model had the best balanced accuracy score?
>
> Which model had the best recall score?
>
> Which model had the best geometric mean score?
>
> What are the top three features?

---

### Hints and Considerations

Use the quarterly data from the LendingClub data that is provided in the `Resources` folder. Keep the file in the zipped format and use the starter code to read the file.

Refer to the [imbalanced-learn](https://imbalanced-learn.readthedocs.io/en/stable/) and [scikit-learn](https://scikit-learn.org/stable/) official documentation for help with training the models. Remember that these models all use the model->fit->predict API.

For the ensemble learners, use 100 estimators for both models.

---

### Submission

* Create Jupyter notebooks for the homework and host the notebooks on GitHub.
* Include a markdown that summarizes your homework and include this report in your GitHub repository.
* Submit the link to your GitHub project to Bootcamp Spot.

---

© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
