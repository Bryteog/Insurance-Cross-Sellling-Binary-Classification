## Insurance Cross Selling Binary Classification
Submission for the Kaggle [Binary Classification on Insurance Cross Selling](https://www.kaggle.com/competitions/playground-series-s4e7) competition.

Three versions were made to track the model improvements (or regression) with changes to aspects of the model.

---------------- 

### V1
The model is a CatBoostClassifier with StratifiedKFold trained for 2 splits.
The Receiver Operating Characteristics (ROC) score obtained is 0.94975.

### V2
The only hyperparameter change is increasing the number of splits to 5. Everything holds constant compared to V1.
The Receiver Operating Characteristics (ROC) score obtained is 0.98091.

### V3
KFold validation was used here in the stead of StratifiedKFold, this was to check the performance when this validation is used because the submission I got my idea from and othersalso implemented this.
The ROC score is 0.98092. So very comparable to the V2.
