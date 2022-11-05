#ROC/AUC

ROC - (receiver operating characteristic curve) Is a graph showing the performance of a classification model at all classification thresholds. This curve plots two parameters

	1. True Positive Rate
		a. TPR = TP / TP + FN
		
	2. False Positive Rate
		a. FPR = FP / FP + TN


An ROC curve plots TRP vs. FPR at different classification thresholds. The better classification threshold will be the one that tanks TPR close to 1 and FRP close to 0.

To compute the points in an ROC curve, we could evaluate a logistic regression model many times with different classification thresholds and in order to visualize this evaluating we can apply a another algorithm called AUC (Area Under the Curve).

AUC provides an aggregate measure of performance across all possible classification thresholds. Maybe that's his name is Area Under the ROC Curve. Thus, the bigger the AUC (close to 1) the better the prediction, otherwise, the close to 0, the worse the prediction.