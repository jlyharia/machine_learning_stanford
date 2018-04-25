# machine_learning_stanford

https://www.coursera.org/learn/machine-learning/home/welcome

http://math.stackexchange.com/questions/477207/derivative-of-cost-function-for-logistic-regression


http://stats.stackexchange.com/questions/79905/cross-validation-including-training-validation-and-testing-why-do-we-need-thr
Why cross-validation need?

The training set is used to choose the optimum parameters for a given model. Note that evaluating some given set of parameters using the training set should give you an unbiased estimate of your cost function - it is the act of choosing the parameters which optimise the estimate of your cost function based on the training set that biases the estimate they provide. The parameters were chosen which perform best on the training set; hence, the apparent performance of those parameters, as evaluated on the training set, will be overly optimistic.

Having trained using the training set, the validation set is used to choose the best model. Again, note that evaluating any given model using the validation set should give you a representative estimate of the cost function - it is the act of choosing the model which performs best on the validation set that biases the estimate they provide. The model was chosen which performs best on the validation set; hence, the apparent performance of that model, as evaluated on the validation set, will be overly optimistic.

Having trained each model using the training set, and chosen the best model using the validation set, the test set tells you how good your final choice of model is. It gives you an unbiased estimate of the actual performance you will get at runtime, which is important to know for a lot of reasons. You can't use the training set for this, because the parameters are biased towards it. And you can't use the validation set for this, because the model itself is biased towards those. Hence, the need for a third set.