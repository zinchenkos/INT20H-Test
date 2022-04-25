![Magnus Sysanus](coollogo_com-22683573.png)
# Magnus Sysanus
## INT20H-2022 TEST TASK
### Driver's Churn

### Assignment
You to build a model that will predict the segment of churn-drivers, ie drivers who will stop using the service.

To do this, you need to teach the model using data from train.csv. After that, using your preprocessing and using your model, you need to assume for each Id from test.csv that the driver belongs to the segment of churn drivers (1 - applies, 0 - does not apply).
Note that it is necessary to predict the fact of the relationship to the churn segment, without reference to the period (week).


### Best result was reached by a model using ensemble of BaggingClassifier and XGBClassifier
BaggingClassifier(base_estimator=XGBClassifier(booster = 'dart', learning_rate=0.4, n_estimators=106, max_depth=3, min_child_weight=0), n_jobs=-1)

### AUC = 0.978

### Ways to improve:
1. To highlight main features, used by model 
1. Reduce data dimension with the help of UMAP, PCA, SVD and display distributions in 2d or 3d space
