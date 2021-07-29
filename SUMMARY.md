# Summary of Risky Business Machine Learning

The following technics are implemented for the assignment, and the results are evaluated.

1. [Resampling](#Resampling)
2. [Ensemble Learning](#Ensemble-Learning)

---

## Resampling

For the Resampling Classification the following algorithms are examined:

1. LogisticRegression without resampling
2. Random Oversampling
3. SMOTE Oversampling
4. Cluster Centroids Undersampling
5. Combination (Over and Under) Sampling using SMOTEENN Algorithm

The results can be summarized as below:

### LogisticRegression without resampling:
- Balanced Accuracy Score: 0.9543211898288821
- Average Recall Score: 0.99
- Geometric Mean Score: 0.95

### Random Oversampling:
- Count of the Target Class: 'low_risk': 56277, 'high_risk': 56277
- Balanced Accuracy Score: 0.9946414201183431
- Average Recall Score: 0.99
- Geometric Mean Score: 0.99

### SMOTE Oversampling:
- Count of the Target Class: 'low_risk': 56277, 'high_risk': 56277
- Balanced Accuracy Score: 0.9946680739911509
- Average Recall Score: 0.99
- Geometric Mean Score: 0.99

### Cluster Centroids Undersampling:
- Count of the Target Class: 'high_risk': 1875, 'low_risk': 1875
- Balanced Accuracy Score: 0.9932813049736127
- Average Recall Score: 0.99
- Geometric Mean Score: 0.99

### Combination (Over and Under) Sampling using SMOTEENN Algorithm:
- Count of the Target Class: 'high_risk': 55652, 'low_risk': 55885
- Balanced Accuracy Score: 0.9946680739911509
- Average Recall Score: 0.99
- Geometric Mean Score: 0.99

---

## Ensemble

For the Ensemble Classification the following scores are measured:

1. Balanced Accuracy Score:
    * The Balanced Random Forest Classifier has Balanced Accuracy Score of 0.7887512850910909, while The Easy Ensemble Classifier has Balanced Accuracy Score of 0.931601605553446. So, obviousely, Easy Ensemble Classifier has better Balanced Accuracy Score.

2. Recall Score:
    * The Balanced Random Forest Classifier has Average Recall Score of 0.87, while The Easy Ensemble Classifier has Average Recall Score of 0.94. So, obviousely, Easy Ensemble Classifier has better Average Recall Score.

3. Geometric Mean Score:
    * The Balanced Random Forest Classifier has Average Geometric Score of 0.78, while The Easy Ensemble Classifier has Average Recall Score of 0.93. So, obviousely, Easy Ensemble Classifier has better Average Geometric Score.

Also, the top three features for the dataset are: `total_rec_prncp`, `total_pymnt` and `total_pymnt_inv`
