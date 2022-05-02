# Credit_Risk_Analysis

![8](https://user-images.githubusercontent.com/94920551/166291744-a03876b6-adfc-40c0-a5ee-1effce78acc7.png)

## Background/Overview
Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## What You're Creating
This new assignment consists of three technical analysis deliverables and a written report. You will submit the following:

* Deliverable 1: Use Resampling Models to Predict Credit Risk
* Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
* Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
* Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

## Results
The Easy Ensemble AdaBoost Classifier is the best of this bunch of models for predicting high-risk credit applications

* Precision: the measure of how reliable a positive classification is. TP/(TP + FP).
  * A low precision is indicative of a large number of false positives (ie. want this to be high)
  * low risk loans: 1.00
  * high risk loans: 0.09
* Recall: the ability of the classifier to find all the positive samples. TP/(TP + FN).
  * A low recall is indicative of a large number of false negatives. (ie. want this to be high)
  * low risk loans: 0.94
  * high risk loans: 0.92
* F1 score: a weighted average of the true positive rate (recall) and precision (best score = 1.0, worst = 0.0)
  * low risk loans: 0.97
  * high risk loans: 0.16
* Support: the number of actual occurrences of the class in the specified dataset.
  * low risk loan: 17,104 actual occurrences
  * high risk loans: 101 actual occurrences

## Summary
One thing to consider would be a false positive result (high risk applicants identified as low risk). This would approve high risk applicants for loans when they should be denied, as they may not be able to pay off their loans. A model with high precision will have lower false positive results. 
Another consideration would be false negative result (low risk applicants identified as high risk). This would deny more people for loans who may have been a good candidate. A model with high recall/sensitivity will have a lower false negative results. 
I would recommend the Easy Ensemble Clasifier model because it resulted in the highest accuracy, precision, and recall/sensitivity values when compared to the other models.
