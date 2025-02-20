# **Logistic Regression**

* Logistic Regression is a supervised learning algorithm used for binary classification problems by predicting the probability that a given input belongs to a particular class.

* Logistic Regression predicts the probability $P(Y=1|X)$ using the logistic (sigmoid) function:

  $P(Y=1|X) = \sigma(W^TX+b)$

  where:

  - $\sigma(z)=1/(1+e^{-z})$ is the sigmoid function;
  - $W$ are the model's weights (coefficients);
  - $X$ is the feature vector;
  - $b$ is the bias term.

* Logistic Regression minimizes the **log loss** (binary cross-entropy):

  $J(W, b) = -\frac{1}{m} \sum_{i=1}^{m} \left[ y_i \log(\hat{y}_i) + (1 - y_i) \log(1 - \hat{y}_i) \right]$

  where:

  - $y_i$ is the actual class label (0 or 1);
  - $\hat{y}_i$ is the predicted probability;
  - $m$ is the total number of training examples.

* We update the parameters $W$ and $b$ using gradient descent;
