# Credit Risk Analysis
## Overview and Purpose
Credit risk can be difficult to predict due to unbalanced classes because the number of good loans typically outweighs the number of risky loans.  The purpose of this project was to apply different machine learning algorithms and models from the imbalanced-learn and scikit-learn libraries to resample data in order to determine which  produced the best outcomes based on the balanced accuracy score, precision score, and recall score for each.  The following were used: 

Oversampling was performed using:
- Random Over Sampler
- SMOTE

Undersampling was performed using:
- Cluster Centroids

Combination of over- and undersampling was perfomed using:
- SMOTEENN

Two models that reduce bias were performed using:
- Balanced Random Forest Classifier
- Easy Ensemble Classifier

## Resources
- Data Source: LoanStats_2019Q1.csv
- Software and Programming Languages: Jupyter Notebook v. 6.4.6; Python v. 3.8.3 :: Anaconda, Inc.; conda v. 4.11.0; imbalanced-learn; scikit-learn v. 0.23.1:: Anaconda, Inc. 


## Results

All models showed extremely low precision (< 0.08) for high risk loans. Recall for most high risk loans ranged from 0.59 to 0.67, except for the Easy Ensemble AdaBoost Classifier where recall was 0.91.  F1 scores for high risk loans ranged from 0.01 to 0.14 across the models tested.  For low risk loans, precision was found to be 1.00 for all models tested but recall ranged from 0.43 to 0.65 for those where data were oversampled, undersampled, or a combinatorial approach was used.  Recall when using the Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier was much improved at 0.91 and 0.94, respectively.  F1 scores for low risk loans ranged from 0.60 to 0.97.  Balanced accuracy scores ranged from 0.51 to 0.925. Individual results were as follows:

- Naive Random Oversampling.  The balanced accuracy score was 0.637.  Precision and recall for high risk loans were 0.01 and 0.62, respectively.  F1 for high risk loans was 0.02.  Precision and recall for low risk loans were 1.00 and 0.65, respectively.  F1 for low risk loans was 0.79 (Fig. 1).

- SMOTE. The balanced accuracy score was 0.630.  Precision and recall for high risk loans were 0.01 and 0.62, respectively.  F1 for high risk loans was 0.02.  Precision and recall for low risk loans were 1.00 and 0.64, respectively.  F1 for low risk loans was 0.78 (Fig. 2).

- Cluster Centroids.  The balanced accuracy score was 0.510.  Precision and recall for high risk loans were 0.01 and 0.59, respectively.  F1 for high risk loans was 0.01.  Precision and recall for low risk loans were 1.00 and 0.43, respectively.  F1 for low risk loans was 0.60 (Fig. 3).

- SMOTEENN.  The balanced accuracy score was 0.630. Precision and recall for high risk loans were 0.01 and 0.62, respectively.   F1 for high risk loans was 0.02.  Precision and recall for low risk loans were 1.00 and 0.64, respectively.  F1 for low risk loans was 0.78 (Fig. 4).

- Balanced Random Forest Classifier.  The balanced accuracy score was 0.787.  Precision and recall for high risk loans were 0.04 and 0.67, respectively. F1 for high risk loans was 0.07.  Precision and recall for low risk loans were 1.00 and 0.91, respectively.  F1 for low risk loans was 0.95 (Fig. 5).

- Easy Ensemble AdaBoost Classifier.  The balanced accuracy score was 0.925.  Precision and recall for high risk loans were 0.07 and 0.91, respectively.  F1 for high risk loans was 0.14. Precision and recall for low risk loans were 1.00 and 0.94, respectively.  F1 for low risk loans was 0.97 (Fig. 6).



__________________________________________________________________________________________________________________________________________________________________
### Naive Random Oversampling

![Naive_random_oversampling](https://user-images.githubusercontent.com/95387273/163584417-d3e66766-012d-4f57-b55d-c4b20ac44146.png)

Fig. 1.  **Naive Random Oversampling.** Confusion matrix, balanced accuracy score, and precision, recall, and F1 scores of the imbalanced classification report for Naive Random Oversampling (0 = high risk, 1 = low risk).

___________________________________________________________________________________________________________________________________________________________________

### SMOTE

![SMOTE_oversampling](https://user-images.githubusercontent.com/95387273/163585602-b166169b-ab24-4cc4-ac9f-a92b128175ff.png)

Fig. 2. **SMOTE**. Confusion matrix, balanced accuracy score, and precision, recall, and F1 scores of the imbalanced classification report for SMOTE (0 = high risk, 1 = low risk). 

___________________________________________________________________________________________________________________________________________________________________

### Cluster Centroids

![Cluster_centroids_undersampling](https://user-images.githubusercontent.com/95387273/163586011-d71bf2cb-0996-4809-ad80-dfbdc0fc9cf1.png)

Fig. 3. **Cluster Centroids.** Confusion matrix, balanced accuracy score, and precision, recall, and F1 scores of the imbalanced classification report for Cluster Centroids (0 = high risk, 1 = low risk).

___________________________________________________________________________________________________________________________________________________________________

### SMOTEENN

![SMOTEENN_combination](https://user-images.githubusercontent.com/95387273/163586539-76daa493-6564-4dab-b1a6-1add20256f92.png)

Fig. 4. **SMOTEENN.** Confusion matrix, balanced accuracy score, and precision, recall, and F1 scores of the imbalanced classification report for SMOTEENN (0 = high risk, 1 = low risk).

___________________________________________________________________________________________________________________________________________________________________

### Balanced Random Forest Classifier

![Balanced_random_forest_classifier](https://user-images.githubusercontent.com/95387273/163587015-43f4e119-72a5-472f-8068-f7a810c5631a.png)

Fig. 5. **Balanced Random Forest Classifier.** Confusion matrix, balanced accuracy score, and precision, recall, and F1 scores of the imbalanced classification report for Balanced Random Forest Classifier (0 = high risk, 1 = low risk).

___________________________________________________________________________________________________________________________________________________________________

### Easy Ensemble AdaBoost Classifier

![Easy_ensemble_AdaBoost_classifier](https://user-images.githubusercontent.com/95387273/163587199-1931d916-1e16-4af2-9255-6c25418c05ce.png)

Fig. 6.  **Easy Ensemble AdaBoost Classifier.** Confusion matrix, balanced accuracy score, and precision, recall, and F1 scores of the imbalanced classification report for Easy Ensemble AdaBoost Classifier (0 = high risk, 1 = low risk). 

____________________________________________________________________________________________________________________________________________________________________

## Summary
Naive Random Oversampling, SMOTE, Cluster Centroids, and SMOTEENN performed similarly in that they all demonstrated a precision of 0.01 for high risk loans and a precision of 1.0 for low risk loans, with mid-range recall scores for high- and low risk loans. F1 values for high risk loans ranged from 0.01 to 0.02, whereas F1 values ranged from 0.60 to 0.79 for low risk loans.  Balanced accuracy scores ranged from 0.51 to 0.637.

The two models that reduce bias, Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier, showed improved results with respect to recall for both high- (especially) and low risk loans, but precision for high risk loans was still <= 0.07 for both.  F1 values for high risk loans were <= 0.14 even though F1 values for low risk loans were >= 0.95. Balanced accuracy scores were >= 0.91 for both.

None of the models are recommended given the extremely low precision values (<= 0.07) for determining high risk loans.   Even though the Easy Ensemble AdaBoost Classifier produced high values for balanced accuracy scores and recall values for high- and low risk loans, the low precision of 0.07 for detecting high risk loan applications renders this an unuseful model. 

