# Module-18-Credit_Risk_Analysis
## Overview of the loan prediction risk analysis:
The purpose of the analysis is to utilize supervised machine learning to help predict credit risk based on a credit card credit dataset. Different resampling techniques are used when evaluating samples such as oversampling (using RandomOverSampler and SMOTE algorithms), undersampling (using ClusterCentroids), and a combination of both (using the SMOTEENN algorithm). In addition, BalancedRandomForestClassifier and EasyEnsembleClassifier, which are machine learning models that reduce bias, were used to predict risk.

## Results:

### 1. Naive Random Oversampling
<img width="705" alt="Screen Shot 2023-02-21 at 7 38 28 PM" src="https://user-images.githubusercontent.com/115126898/220491100-2d72245d-d46f-48ef-b5fd-96fe1f00706f.png">

- balanced accuracy score is 65%
- precision score for high-risk is at 1%, and precision for low-risk is at about 100%
- recall score for high-risk is 72% and for low-risk is 59%. Average/total recall is 59%

### 2. SMOTE Oversampling
<img width="705" alt="Screen Shot 2023-02-21 at 7 39 14 PM" src="https://user-images.githubusercontent.com/115126898/220491146-53e354ba-0a30-46cf-9c8f-7f875d01635c.png">

- balanced accuracy score is 66%
- precision score for high-risk is at 1%, and precision for low-risk is at about 100%
- recall score for high-risk is 63% and for low-risk is 69%. Average/total recall is 69%

### 3. Undersampling
<img width="705" alt="Screen Shot 2023-02-21 at 7 39 29 PM" src="https://user-images.githubusercontent.com/115126898/220491225-f760432c-8205-4200-a9de-1bd4f91c7381.png">

- balanced accuracy score is 54%
- precision score for high-risk is at 1%, and precision for low-risk is at about 100%
- recall score for high-risk is 69% and for low-risk is 40%. Average/total recall is 40%

### 4. Combination (Over and Under) Sampling
<img width="705" alt="Screen Shot 2023-02-21 at 7 39 40 PM" src="https://user-images.githubusercontent.com/115126898/220491288-f497a80c-af33-41fe-a3e9-8ba551a38e8c.png">

- balanced accuracy score is 65%
- precision score for high-risk is at 1%, and precision for low-risk is at about 100%
- recall score for high-risk is 72% and for low-risk is 57%. Average/total recall is 57%

## Resampling using Ensembles

### 5. Balanced Random Forest Classifier
<img width="705" alt="Screen Shot 2023-02-21 at 8 26 05 PM" src="https://user-images.githubusercontent.com/115126898/220497017-549576c1-0d38-4ea0-a37a-f5d8906d1da7.png">

- balanced accuracy score is 79%
- precision score for high-risk is at 3%, and precision for low-risk is at about 100%
- recall score for high-risk is 70% and for low-risk is 87%. Average/total recall is 87%

### 6. Easy Ensemble AdaBoost Classifier
<img width="705" alt="Screen Shot 2023-02-21 at 8 26 19 PM" src="https://user-images.githubusercontent.com/115126898/220497037-2eaab54d-f8d3-465e-8a2f-c510df5526a9.png">

- balanced accuracy score is 93%
- precision score for high-risk is at 9%, and precision for low-risk is at 100%
- recall score for high-risk is 92% and for low-risk is 94%. Average/total recall is 94%


## Summary:
Based on the results above, the Easy Ensemble AdaBoost Classifier is the best model to use with the highest balanced accuracy score of 93% and recall score of 94%. In both these categories, the closer to 100%, the better the model. The precision score for all the models were pretty similar and within close range to one another. 



