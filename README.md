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

All models showed extremely low precision (< 0.08) high risk loans. Recall for high risk loans ranged form   ...

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
