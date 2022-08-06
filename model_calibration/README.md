# Model Calibration

All ML algorithms must have some level of calibration in their parameters when we want to achieve better accuracy for our models.

To achieve good accuracy we need to think about how many times we need to run the model and how many values of one or more parameters we need to cross in order to get a best result.

As a scientist we can't do it manually because the volume of data can be very large and it's hard to say if it's a good strategy.

So we need to think of algorithms that do this automatically for us. For example:

## Randomized Search
This function implements a randomized search over parameters, where each setting is sampled from a distribution over possible parameter values.

## Grid Search CV
This function is similar to the Randomized Search, the only difference is that while Randomized Search CV performs a limited numbers of iterations the Grid Search CV combines all possible parameter values. 
