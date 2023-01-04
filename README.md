# Credit_Risk_Analysis

## Overview of the analysis: 

In this analysis we use Python to build and evaluate several machine learning models to predict credit risk. Being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and  provide recommendations on what to do in cases of fraud. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we employed different techniques to train and evaluate models with unbalanced classes. 

Tools used in the analysis:
- Pandas and Matplotlib
- Numpy library
- Imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling
- Credit card credit dataset from LendingClub
- Oversample the data using the RandomOverSampler and SMOTE algorithms
- Undersample the data using the ClusterCentroids algorithm
- Combinatorial approach of over- and undersampling using the SMOTEENN algorithm
- BalancedRandomForestClassifier and EasyEnsembleClassifier to reduce bais

## Results: 

### RandomOverSampler model

![oversampling](https://user-images.githubusercontent.com/111251560/210569078-09059bb8-d2ec-4f7c-b037-a07811582986.png)


### SMOTE model

![SMOT_oversampling](https://user-images.githubusercontent.com/111251560/210569132-9026ea2b-7915-43d7-ad2a-5882da9430e9.png)


### ClusterCentroids model

![undersampling](https://user-images.githubusercontent.com/111251560/210569386-3defdd61-bcc0-46be-b631-9d2aa62e7343.png)


### SMOTEENN model

![combination(over and under) sampling](https://user-images.githubusercontent.com/111251560/210569486-d990f73a-c002-4c4e-b61d-b29f02e718f9.png)


### BalancedRandomForestClassifier model

![balanced_random_forest](https://user-images.githubusercontent.com/111251560/210569578-6e5a980a-d8f8-4ada-aaae-ddd87a884dd8.png)


### EasyEnsembleClassifier model

![eea_classifier](https://user-images.githubusercontent.com/111251560/210569638-7271b397-9a2f-443e-82f0-084f41bed981.png)


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
