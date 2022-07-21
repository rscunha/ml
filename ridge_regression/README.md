# Ridge Regression

When we are talking about Linear Regression we are talking about drawing a line. The mathematical calculation to draw this line does not care if the variables used to perform the calculation have a large variation in size between them, I mean, if one of them is much larger than the others.

But when we speak about Ridge Regression, we need apply a regularization mechanism so that the variables have the same weight for the calculation and with that our Machine Learning Model can be more general.

This mechanism is a mathematical formula that makes the calculation more "blind" in relation to the training data and thus helps our model not suffer from overfitting.

The Ridge algorithm formula: ||y - Xw||^2_2 + alpha * ||w||^2_2