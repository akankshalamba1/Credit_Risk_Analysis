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

#### Outcome:
- The balanced accuracy score is 63%.
- The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
- The low_risk population is too high, its precision is almost 100% with a sensitivity of 65%.

### SMOTE model

![SMOT_oversampling](https://user-images.githubusercontent.com/111251560/210569132-9026ea2b-7915-43d7-ad2a-5882da9430e9.png)

#### Outcome:

- The balanced accuracy score is 63%.
- The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
- The low_risk population is too high, its precision is almost 100% with a sensitivity of 64%.

### ClusterCentroids model

![undersampling](https://user-images.githubusercontent.com/111251560/210569386-3defdd61-bcc0-46be-b631-9d2aa62e7343.png)

#### Outcome:

- The balanced accuracy score is 52%.
- The high_risk precision is about 1% only with 61% sensitivity which makes a F1 of 1% only.
- The low_risk population has high false positive, its precision is almost 100% with a sensitivity of 45%.

### SMOTEENN model

![combination(over and under) sampling](https://user-images.githubusercontent.com/111251560/210569486-d990f73a-c002-4c4e-b61d-b29f02e718f9.png)

#### Outcome:

- The balanced accuracy score is 62%.
- The high_risk precision is about 1% only with 71% sensitivity which makes a F1 of 2% only.
- The low_risk population is large, its precision is almost 100% with a sensitivity of 54%.

### BalancedRandomForestClassifier model

![balanced_random_forest](https://user-images.githubusercontent.com/111251560/210569578-6e5a980a-d8f8-4ada-aaae-ddd87a884dd8.png)

#### Outcome:

- The balanced accuracy score is 78%.
- The high_risk precision is about 4% only with 67% sensitivity which makes a F1 of 7%.
- The low_risk population has large number of true negative, its precision is almost 100% with a sensitivity of 91%.

### EasyEnsembleClassifier model

![eea_classifier](https://user-images.githubusercontent.com/111251560/210569638-7271b397-9a2f-443e-82f0-084f41bed981.png)


#### Outcome:

- The balanced accuracy score is 92%.
- The high_risk precision is about 7% only with 91% sensitivity which makes a F1 of 14%.
- The low_risk population has largest number of true negative, which means that 16139 of the credits were predicted low-risk and were actually low-risk, its precision is 100% with a sensitivity of 94%.

## Summary:

All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits. The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. On the other hand, even if the EasyEnsembleClassifier model has the highest precision level as compared to other models i.e. 7%, but for the analysis precision is too low, which means a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities. 

For those reasons I would not recommend the bank to use any of these models to predict credit risk.
