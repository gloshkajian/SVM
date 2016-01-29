A Linear Support Vector Machine
===

This is an implementation of a linear support vector machine in Python, a supervised learning model used to non-probabilistically classify multidimensional datasets. For this project, I used Lutz Hamel's "Knowledge Discovery with Support Vector Machines" (2009, Univ. of Rhode Island), which is an excellent introduction to SVMs. I took on this project as a personal learning experience, so that I might gain a deeper understanding of how this kind of classifier works (both mathematically and programmatically), which would assist me in working with pre-built SVMs, such as that of Scikit-Learn, and perhaps even fine-tuning these models later.

Currently, this SVM only supports linearly separable datasets, and thus only has a linear kernel function (f(x1, x2) = x1 dot x2). I plan to eventually incorporate polynomial, Gaussian, and RBF kernel functions, and provide support for datasets with 3+ features (i.e. higher-dimensional sets). There are other factors, such as slack variables for soft margins, or replacing CVXOPT's quadratic solver with the standard sequential minimal optimization. This version of an SVM demonstrates:

1) Finding maximum-margin decision boundaries and supporting hyperplanes through convex optimization.

2) Fitting the SVM to a linearly separable training dataset, and predicting the labels of a testing dataset. 

3) Dynamically plotting the results using Matplotlib's animation module.

Note: All data is randomly generated using NumPy's random.multivariate_normal() function.