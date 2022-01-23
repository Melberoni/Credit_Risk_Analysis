# Credit_Risk_Analysis

## Overview
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we will predict credit card risk using multiple methods. I will build and evaluate logistic regression models using resampling the methods to compare are oversampling with SMOTE and RandomOverSampler, undersampling with ClusterCentroids, combinatorial approach using SMOTEENN. In addition, i will use two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results
### Random Oversampling
* Balanced Accuracy Score was low. 
* The precision was high, but the recall was low 
* ![random_oversampling](https://github.com/Melberoni/Credit_Risk_Analysis/blob/1cbefb12442b9ec189ceccfd838736ded77313c1/images/random_overSampler_results.png)

### SMOTE oversampling
* Balanced accuracy score was like random oversampling. 
* the precision was high, and the recall was higher than random oversampling. 
* This did slightly better than random oversampling.
* ![SMOTE oversampling](https://github.com/Melberoni/Credit_Risk_Analysis/blob/1cbefb12442b9ec189ceccfd838736ded77313c1/images/smote_results.png)

### Cluster Centroids undersampling
* Balanced accuracy score was worse than oversampling
* precision was the same as both oversampling methods, but recall was worse. 
* overall, this  model did worse than both the oversampling methods
* ![ClusterCentroids_undersampling](https://github.com/Melberoni/Credit_Risk_Analysis/blob/1cbefb12442b9ec189ceccfd838736ded77313c1/images/cluster_centroids_results.png)

### Combined SMOTEENN sampling
* Balanced accuracy score was very similar to the oversampling
* Precision was same as the above methods, but recall was worse than oversampling methods but slightly better than oversampling methods
* overall, this model did better than undersampling but worse than oversampling
* ![SMOTEENN_sampling](https://github.com/Melberoni/Credit_Risk_Analysis/blob/1cbefb12442b9ec189ceccfd838736ded77313c1/images/smoteenn_results.png)

### Balanced Random Forest Classifier
* Balanced accuracy score was much better than the above sampling methods
* the precision was the same as everything else and the recall was better than all the above sampling methods
* overall, this model did better than all the sampling methods above with an f1 score of .93
* ![Balanced RandomForest](https://github.com/Melberoni/Credit_Risk_Analysis/blob/1cbefb12442b9ec189ceccfd838736ded77313c1/images/BalancedRandomForest_results.png)

### Easy Ensemble AdaBoost Classifier
* The balanced accuracy score was the best so far at .93
* the precision again is the same as all other methods, but the recall is much better than anything else we have seen yet at .94 overall.
* Overall, this method looks like it does the best with an f1 score of .97, and it has the fewest type 1 and type 2 errors.
* ![EEABC](https://github.com/Melberoni/Credit_Risk_Analysis/blob/1cbefb12442b9ec189ceccfd838736ded77313c1/images/adaBoost_results.png)

## Summary
Overall, the models that reduced bias worked much better than over or under sampling. Oversampling worked better than undersampling.
I would recommend using the Easy Ensemble AdaBoost Classifier over any of the other models because it had the best F1 score and reduced the type 1 and type 2 errors the most compared to all other models.
