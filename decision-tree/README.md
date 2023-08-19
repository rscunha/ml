# Decision Tree

This is also a classification algorithm that create a structure that remind a tree, because of the relationship between of the data. The target variable need to be evaluate based on their branchs (childs) where we'll decided which better path to follow until we can know the best outcome of the data analisy.

![Decision Tree]("./img.png")

To create the structure of a decision tree we can use the formula of Information gain, that is a decrease in entropy. So in the group of data, those that have the best gain of information will be the first branch of the tree, so that, follow for the next variable that had the second best value for the information gain.

Entropy Formula
- E = -∑ p(i) * log2 p(i)

Information Gain Formula
- IG = Entropy(father) -∑ (weith.f * Entropy(child))
