# Regularization

The previous repoitory saw the Curse of Dimensionality. This repository is kind of a solution to the Curse of Dimensionality.
As the data points on adding varius features, becomes too clustered to make a classification by a classifier. 

What Regularization does is that for all the beta coefficients of an estimator, it decreases or shrinks the magnitude of the beta coefficent. Simultaneously the cost function is penalised with the product of (alpha x beta(i)^2). The alpha is known as the power
of regularization.

Ridge and Lasso regression does the same regularization for every regressor. These methods are based on regularization.

Important notes:

1. Value of alpha must always originate from a logspace interval. (Example: np.logspace(-2,2,100).

2. Always scale the data prior to regularization.

Important learnings:

1. Lasso automatically does feature selecton by, i.e, pushing the beta coefficient to zero, hence the importance of that particular feature is diminished. 

2. Ridge on the other hand, pushes it's beta coefficients to nearly ero and not exactly zero.

Following graph shows 'R_2 score vs. Alpha':

![reg1](https://user-images.githubusercontent.com/55191934/76686486-c4453a00-6641-11ea-81f5-a8f6fc6081fd.PNG)
