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


### SMOTE model


### ClusterCentroids model


### SMOTEENN model


### BalancedRandomForestClassifier model


### EasyEnsembleClassifier model

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
