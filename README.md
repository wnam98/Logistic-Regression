# Binary Classification of a Microchip Dataset using Logistic Regression
Suppose you are the product manager of the factory and you have the test results for some microchips on two different tests i.e 𝑥1 and 𝑥2. From these two tests, you would like to determine whether the microchips should be accepted or rejected. To help you make the decision, you have a dataset of test results on past microchips, from which you can build a logistic regression model. The scatter plot of training data is as shown below. Note features have been normalized.

![microchips](https://raw.github.com/wnam98/Logistic-Regression/master/imgs/microchips.PNG "microchips")

Logisitic Regression is used to model the probability of a feature belonging to a certain class (in this case, pass/fail). Each object would be assigned a probability between 0 and 1 and a discriminant function would group the features to the appropriate classes. The basic model is displayed below:

![log_reg](https://raw.github.com/wnam98/Logistic-Regression/master/imgs/log_reg.png "log_reg")

where Y denotes the set of classes {0,1} and x is the feature vector of attributes [𝑥1, 𝑥2]. A total of three weights were trained with batch gradient descent and fed into the sigmoid activation function, with the discriminant function placing features with P >= .5 into class 1. Training accuracy yielded less than 50% because the data is not lineary classifiable. To better fit the data, more features were created for each data point, adding more basis equations to the weighted sum with degrees up to the 6th power. As a result, the input data has transformed into a matrix spanning 28-dimensions. 

## Regularization

While a higher dimensional phi is a more accurate classifier, it is susceptible to overfitting and would yield low testing accuracy. Therefore, a regularized regression model would be required, along with a weight penalizer in the gradient descent algorithm. The regularization of choice is L2 ridge regression which adds a squared magnitude of coefficient as penalty term to the loss function. The model is displayed below:

![l2](https://raw.github.com/wnam98/Logistic-Regression/master/imgs/l2.PNG "l2")
