# Credit_Risk_Analysis

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

- Random Oversampling

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/RandomOversampling.png" width="85%"/>
</p>

- SMOTE Oversampling

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/SMOTEoversampling.png" width="85%"/>
</p>

- Cluster Centroids Undersampling

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroidUndersampling.png" width="85%"/>
</p>

-  SMOTEENN Combination (Over and Under) Sampling

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/CombinationSampling.png" width="85%"/>
</p>

- Balanced Random Forest Classifier Ensemble Classifier

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.png" width="85%"/>
</p>

- Easy Ensemble AdaBoost Classifier

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.png" width="85%"/>
</p>

## Summary

The confusion matrix can read as such:

<p align="center">  
<img src="https://github.com/mcgibbenyd1/Credit_Risk_Analysis/blob/main/Resources/Confusion.png" width="85%"/>
</p>

Precision = TP/(TP + FP) = a measure of how reliable a positive classification is. 

Sensitivity = TP/(TP + FN) =  a measure of how reliable the correct classification is choosen

- pre (precision), rec (sensitivity) and f1 are the results being used to evaluate each method for the Credit Card Risk.

1) Random Oversampling
	
	- Based on the High Risk Category the precision was very low at about 1% and f1 score of 2% meaning there is not a good balencing in the actual to predicted

2) SMOTE Oversampling

	- Overall the averages increased in favor of the low risk category with precision going up 2%  but has the best balencing of the over and under sampling methods. 

3) Cluster Centroids Undersampling

	- Undersampling proved to be a worse prediction with an average f1 score of 56% and favoring precision over sensitivity.

4) SMOTEENN Combination (Over and Under) Sampling

	- Between the Over and under sampling the combination does not quite match the SMOTE sampling method with 72 % for f1 score to the SMOTE 81%to the SM

5) Balanced Random Forest Classifier Ensemble Classifier

	- The Sensitivity is higher for this method with a good balancing at 93%

6) Easy Ensemble AdaBoost Classifier

	- This is the best prediction of the 6 methods with a high sensitivity and precision with a minimal number of false negatives