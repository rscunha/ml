# KNN Algorithm

The K-nearest neighbors is the algorithm used to classify a new group of data after an another group have ever been classified, in this case we are talking about the training data. Its logic consists in to find the nearest K after a new group of data being show up to the model.

For example:

Knowing we already have two groups of classified data, we now want to classify a new data group. To do it using the KNN algorithm we'll need to set a threshold called K to a value that indicates the number of k-nearest neighbors that the algorithm needs to calculate to know which group of data already classified does it belong to the new informed data.  An important detail here is that the new data will be sorted to the group with the highest number of elements discovered among the k-nearest neighbors.

IMPORTANT

As the kNN algorithm processes a calculation between all the  variables, it is a best practice that all the predictor variables are normalized, because as the calculation is performed in a hyperspace, the values can be very different from each other and, therefore, the model may suffer some negative interference.

As the kNN algorithm processes a calculation between all the variables, it is a good practice that all the predictor variables are normalized, because as the calculation is performed in a hyperspace, the values can be very different from each other and, therefore, the model may suffer some negative interference. .