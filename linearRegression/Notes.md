Linear Regression:

Y = mx+ c 
Linear regression is a linear model, e.g. a model that assumes a linear relationship between the input variables (x) and the single output variable (y). More specifically, that y can be calculated from a linear combination of the input variables (x).

When a coefficient becomes zero, it effectively removes the influence of the input variable on the model and therefore from the prediction made from the model (0 * x = 0). This becomes  relevant if you look at regularization methods that change the learning algorithm to reduce the complexity of regression models by putting pressure on the absolute size of the coefficients, driving some to zero.

Ordinary Least Squares 
* It is a technique to prepare or train linear regression equation from data.

* The Ordinary Least Squares procedure seeks to minimize the sum of the squared residuals. This means that given a regression line through the data we calculate the distance from each data point to the regression line, square it, and sum all of the squared errors together. This is the quantity that ordinary least squares seeks to minimize.

Gradient Descent
* works by starting with random values for each coefficient. The sum of the squared errors are calculated for each pair of input and output values. A learning rate is used as a scale factor and the coefficients are updated in the direction towards minimizing the error. The process is repeated until a minimum sum squared error is achieved or no further improvement is possible.
* When using this method, you must select a learning rate (alpha) parameter that determines the size of the improvement step to take on each iteration

Regularization

* Process of adding something to solve ill posed problems.
* Lasso Regression: where Ordinary Least Squares is modified to also minimize the absolute sum of the coefficients (called L1 regularization).
* Ridge Regression: where Ordinary Least Squares is modified to also minimize the squared absolute sum of the coefficients (called L2 regularization).

Preparation of Data

- Linear Assumption : Linear regression assumes that the relationship between your input and output is linear. It does not support anything else.
- Remove Noise. Linear regression assumes that your input and output variables are not noisy. 
- Remove Collinearity. Linear regression will over-fit your data when you have highly correlated input variables
- Gaussian Distributions. Linear regression will make more reliable predictions if your input and output variables have a Gaussian distribution. 
- Rescale Inputs: Linear regression will often make more reliable predictions if you rescale input variables using standardization or normalization.

Function for Gradient descent  :
Y = b0 + b1 * x
Stochastic gradient descent requires two parameters:
* Learning Rate: Used to limit the amount each coefficient is corrected each time it is updated.
* Epochs: The number of times to run through the training data while updating the coefficients.
