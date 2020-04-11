# Binary Classification of a Microchip Dataset using Logistic Regression
Suppose you are the product manager of the factory and you have the test results for some microchips on two different tests i.e 𝑥1 and 𝑥2. From these two tests, you would like to determine whether the microchips should be accepted or rejected. To help you make the decision, you have a dataset of test results on past microchips, from which you can build a logistic regression model. The scatter plot of training data is as shown below. Note features have been normalized.

![microchips](https://raw.github.com/wnam98/Logistic-Regression/master/imgs/microchips.PNG "microchips")

Logisitic Regression is used to model the probability of a feature belonging to a certain class (in this case, pass/fail). Each object would be assigned a probability between 0 and 1 and a discriminant function would group the features to the appropriate classes. The basic model is displayed below:

![log_reg](https://raw.github.com/wnam98/Logistic-Regression/master/imgs/log_reg.png "log_reg")
