## Ridge Regression(L2 Regression)

### Aim - It is Mainly Used to Reduce the Overfitting Condition 

1. Overfitting Condition - Overfitting occurs when the model learns the training data too perfectly, including noise and random fluctuations.It performs very well on training data but poorly on unseen data.

* Example   
     
     * Train Accuracy = 90%
     * Test Accuracy =  70%

In Both the cases we can conclude that the model high Variance and Low Bias
* Note: When we get the difference between actual value and predicted value as 0 then It is considered as overfitted condition


2. Underfitting Condition - Underfitting occurs when the model is too simple to learn the patterns in the data. The model fails to perform well on both training and testing data.

* Example 

   * Train Accuracy = 60%
   * Test Accuracy = 62%

From Above we can say that model has high bias and high variance 

### Ultimate Goal - Build a generalized model that has Low Bias and Low Variance 

* i.e Train Accuracy = 90% and Test Accuracy = 89%

* Equation is defined as:

$$J(\theta) = \frac{1}{2m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})^2 + \lambda \sum_{j=1}^{n} \theta_j^2$$

**Benifit- Overfitting Condition is Removed**

*** 
## Lasso Regression(L1 Regression)

* **It is mainly used for feature selection and reduce overfitting condition as well**

$$J(\theta) = \frac{1}{2m} \sum_{i=1}^{m} (h_\theta(x^{(i)}) - y^{(i)})^2 + \lambda \sum_{j=1}^{n} |\theta_j|$$

* **It Shrinks the coefficient or reduce corelation and helps in feature selection**


***

## Elastic Net Regression

* **It is used for Reducing the Overfitting Problem and helps in feature Selection**

$$Cost = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 +\lambda \sum_{j=1}^{n} \theta_j^2+ \lambda \sum_{j=1}^{n} |\theta_j|$$









