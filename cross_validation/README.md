# Cross Validation

Cross-validation is a technique for separating data between training and test to compare performance between linear models.

The technique consists of splitting the data into a number of folds with the same amount of data in each fold and running the algorithm using each fold of data as a block of train and test data.

For example:

|FOLD 1|FOLD 2|FOLD 3|FOLD 4|FOLD 5|
|------|------|------|------|------|
|**TEST**|TRAIN|TRAIN|TRAIN|TRAIN|
|TRAIN|**TEST**|TRAIN|TRAIN|TRAIN|
|TRAIN|TRAIN|**TEST**|TRAIN|TRAIN|
|TRAIN|TRAIN|TRAIN|**TEST**|TRAIN|
|TRAIN|TRAIN|TRAIN|TRAIN|**TEST**|

The table above shows five folds (k=5) which are the data blocks  used to validate the regression model.

As we can see the Cross-validation algorithm will use each data block in a fold as a training and test to make it more generalized.
 
The result of each fold execution is the R2 evaluation and the final result is the average (mean) for each R2 evaluation.