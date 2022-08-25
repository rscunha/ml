# Confusion Matrix

When we are talking about evaluation of accuracy from a Logistic Regression Model we can't obtain only the score (R2 Coef) as a key indicator because perhaps the distribution of the data of the target classes found may be unbalanced between them.

For example:

Imagine a target class that have two values, 0 and 1 in a set of 1000 data rows. Now imagine that we have in this sample a total of 900 lines of value 0 and 100 of value 1.

In this case we have a big data unbalanced between the values and maybe our Logistic Regression Model gave us a high score but, unnecessary a right score. 

This is because if our model assigns all values as 0, for example, we don’t need a Machine Learning Model because we would know that the result will be 0 and we would know because 0 is the largest value among the sample.

Because of this, we need to apply a technique called Confusion Matrix:

The best way to explain it is by showing the table bellow:

![Confusion Matrix][confusion_matrix.png]

The image above show us all possibilities that Machine Learning Model can evaluate for us.

So, when we have a large volume of unbalanced data in the Logistic Regression Model we need to run a Confusion Matrix to know how much data was right in prediction