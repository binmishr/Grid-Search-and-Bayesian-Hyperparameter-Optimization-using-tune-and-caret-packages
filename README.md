# Grid-Search-and-Bayesian-Hyperparameter-Optimization-using-tune-and-caret-packages



Hyperparameter Optimization Methods
=======================================

In contrast to the model parameters, which are discovered by the learning algorithm of the ML model, the so called Hyperparameter(HP) are not learned during the modeling process, but specified prior to training.

Hyperparameter tuning is the task of finding optimal hyperparameter(s) for a learning algorithm for a specific data set and at the end of the day to improve the model performance.

There are three main methods to tune/optimize hyperparameters:

a) Grid Search method: an exhaustive search (blind search/unguided search) over a manually specified subset of the hyperparameter space. This method is a computationally expensive option but guaranteed to find the best combination in your specified grid.

b) Random Search method: a simple alternative and similar to the grid search method but the grid is randomly selected. This method (also blind search/unguided search) is faster at getting reasonable model but will not get the best in your grid.

c) Informed Search method:
In informed search, each iteration learns from the last, the results of one model helps creating the next model.

The most popular informed search method is Bayesian Optimization. Bayesian Optimization was originally designed to optimize black-box functions. 

In this post, we will focus on two methods for automated hyperparameter tuning, Grid Search and Bayesian optimization.
We will optimize the hyperparameter of a random forest machine using the tune library and other required packages (workflows, dials. ..). 
