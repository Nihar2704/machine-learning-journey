## Linear Regression

**Linear Regression is a method used to find the relationship between an input and an output by drawing the best-fit straight line through the data points.**

### Things to Remember Before Solving Any Problem

1. Know What exactly is the problem we are solving
2. Know Geometric Intuition
3. Know about the Mathematical Intuition

### AIM:
**The Aim is to find the best fit line with minimum curve**

### Equation Of Line
***
* Equation of line = **y=mx+c**
   * m = slope of line
   * c = intercept
#### Hypothesis: A hypothesis is a statement or assumption that we make before testing with data.

For Linear Regression, the hypothesis is: 
       **$$h_\theta(x) = \theta_0 + \theta_1 x$$**

#### We have to select One best fit line in such a way that error must be less, so we need cost function

#### Cost Function: A Cost Function is a formula that tells us how wrong our machine learning model's predictions are.

Cost function is defined as:

$$J(\theta_0, \theta_1) = \frac{1}{2m} \sum_{i=1}^{m} \left( h_\theta(x^{(i)}) - y^{(i)} \right)^2$$

## Repeat Convergence Theorem

Repeat Until Convergence is a process where the model keeps adjusting its parameters again and again until it reaches the best possible values and the error becomes minimum.

$$\theta_j := \theta_j - \alpha \frac{\partial}{\partial \theta_j} J(\theta_0, \theta_1, \dots, \theta_n)$$

#### Learning Rate: Learning Rate is a value that determines how big a step the model takes while trying to reduce the cost function. 

### OUTLINE
***
**1. Start with some value of θ<sub>0</sub> and θ<sub>i</sub>**

**2. Keep Changing the value to reduce J(θ<sub>0</sub> and θ<sub>i</sub>) untill we reach near global minima**

**3. Apply Convergence Theorem**
​
 