# Summary of 4_Default_Xgboost

[<< Go back](../README.md)


## Extreme Gradient Boosting (Xgboost)
- **n_jobs**: -1
- **objective**: multi:softprob
- **eta**: 0.075
- **max_depth**: 6
- **min_child_weight**: 1
- **subsample**: 1.0
- **colsample_bytree**: 1.0
- **eval_metric**: mlogloss
- **num_class**: 8
- **explain_level**: 2

## Validation
 - **validation_type**: split
 - **train_ratio**: 0.75
 - **shuffle**: True
 - **stratify**: True

## Optimized metric
logloss

## Training time

21.7 seconds

### Metric details
|           |        0 |   1 |        2 |   3 |        4 |   5 |        6 |        7 |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|---------:|----:|---------:|----:|---------:|----:|---------:|---------:|-----------:|------------:|---------------:|----------:|
| precision | 1        |   0 | 0.285714 | 0.2 | 0.416667 | 0.4 | 0.444444 | 0.666667 |   0.444444 |    0.426687 |       0.385626 |   1.66433 |
| recall    | 0.8      |   0 | 0.333333 | 0.2 | 1        | 0.4 | 0.8      | 0.4      |   0.444444 |    0.491667 |       0.444444 |   1.66433 |
| f1-score  | 0.888889 |   0 | 0.307692 | 0.2 | 0.588235 | 0.4 | 0.571429 | 0.5      |   0.444444 |    0.432031 |       0.390865 |   1.66433 |
| support   | 5        |   9 | 6        | 5   | 5        | 5   | 5        | 5        |   0.444444 |   45        |      45        |   1.66433 |


## Confusion matrix
|              |   Predicted as 0 |   Predicted as 1 |   Predicted as 2 |   Predicted as 3 |   Predicted as 4 |   Predicted as 5 |   Predicted as 6 |   Predicted as 7 |
|:-------------|-----------------:|-----------------:|-----------------:|-----------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| Labeled as 0 |                4 |                0 |                0 |                0 |                0 |                0 |                1 |                0 |
| Labeled as 1 |                0 |                0 |                4 |                1 |                4 |                0 |                0 |                0 |
| Labeled as 2 |                0 |                0 |                2 |                2 |                1 |                1 |                0 |                0 |
| Labeled as 3 |                0 |                0 |                0 |                1 |                1 |                2 |                1 |                0 |
| Labeled as 4 |                0 |                0 |                0 |                0 |                5 |                0 |                0 |                0 |
| Labeled as 5 |                0 |                0 |                1 |                1 |                1 |                2 |                0 |                0 |
| Labeled as 6 |                0 |                0 |                0 |                0 |                0 |                0 |                4 |                1 |
| Labeled as 7 |                0 |                0 |                0 |                0 |                0 |                0 |                3 |                2 |

## Learning curves
![Learning curves](learning_curves.png)

## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Precision Recall Curve

![Precision Recall Curve](precision_recall_curve.png)



## SHAP Importance
![SHAP Importance](shap_importance.png)

## SHAP Dependence plots

### Dependence 0 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_0.png)
### Dependence 1 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_1.png)
### Dependence 2 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_2.png)
### Dependence 3 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_3.png)
### Dependence 4 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_4.png)
### Dependence 5 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_5.png)
### Dependence 6 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_6.png)
### Dependence 7 (Fold 1)
![SHAP Dependence from fold 1](learner_fold_0_shap_dependence_class_7.png)

## SHAP Decision plots

### Worst decisions for selected sample 1 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_0_worst_decisions.png)
### Worst decisions for selected sample 2 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_1_worst_decisions.png)
### Worst decisions for selected sample 3 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_2_worst_decisions.png)
### Worst decisions for selected sample 4 (Fold 1)
![SHAP worst decisions from Fold 1](learner_fold_0_sample_3_worst_decisions.png)
### Best decisions for selected sample 1 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_0_best_decisions.png)
### Best decisions for selected sample 2 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_1_best_decisions.png)
### Best decisions for selected sample 3 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_2_best_decisions.png)
### Best decisions for selected sample 4 (Fold 1)
![SHAP best decisions from Fold 1](learner_fold_0_sample_3_best_decisions.png)

[<< Go back](../README.md)
