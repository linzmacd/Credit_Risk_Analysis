# Credit Risk Analysis

## Overview

Due to the nature of credit risk, there is an inherent unbalanced classification problem when developing predictive models. The purpose of this analysis was to train and test six machine learning models that use different sampling methods, and to  evaluate each model based on its balanced accuracy, precision, and recall scores.

## Results

The balanced accuray scores and classification reports for the six machine learning method tested are listed below:

- Naive Random Oversampling - Balanced Accuracy Score 0.6603

<img src="https://github.com/linzmacd/Credit_Risk_Analysis/blob/main/Resources/ros.PNG" width="50%">

- SMOTE Oversampling - Balanced Accuracy Score 0.6537

<img src="https://github.com/linzmacd/Credit_Risk_Analysis/blob/main/Resources/smote.PNG" width="50%">

- Cluster Centroid Undersampling - Balanced Accuracy Score 0.5443

<img src="https://github.com/linzmacd/Credit_Risk_Analysis/blob/main/Resources/cc.PNG" width="50%">

- SMOTEENN Combination Sampling - Balanced Accuracy Score 0.6448

<img src="https://github.com/linzmacd/Credit_Risk_Analysis/blob/main/Resources/smoteenn.PNG" width="50%">

- Balanced Random Forest - Balanced Accuracy Score 0.7885

<img src="https://github.com/linzmacd/Credit_Risk_Analysis/blob/main/Resources/brf.PNG" width="50%">

- Easy Ensemble AdaBoost - Balanced Accuracy Score 0.9317

<img src="https://github.com/linzmacd/Credit_Risk_Analysis/blob/main/Resources/ee.PNG" width="50%">

## Summary

The ensemble machine learning methods outperform the statistical oversampling and undersampling methods, both having f1 scores over 0.9. Of the two ensemble methods, the Easy Ensemble Adaboost classifier has the higher balanced accuracy score of 0.93 and higher precision and recall scores than the Balanced Random Forest classifier, making it the best performing model we tested.

However, the Easy Ensemble Adaboost classifier isn't a perfect predictive model and has its drawbacks. While the precision for the majority class and the recall (sensitivity) for both classes are high, the precision for the minority class is still quite low at 0.09. This means that while we are catching 92% of the true high-risk credit applicants, 91% of our rejections are going to actual low-risk applicants. Though low, this precision score is still the highest among the models we tested, so we would still recommend using this model out of those tested. 
