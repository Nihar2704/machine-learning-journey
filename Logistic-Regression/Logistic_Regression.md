## Logistic Regression
Logistic Regression is a supervised machine learning algorithm used for classification problems, where the goal is to predict the probability that an observation belongs to a particular class.

**Logistic Regression works really well for binary classificaton**

#### Why Linear Regression is not good:
* You cannot solve a classification problem with linear regression beacacuse if outlier exist then the best fit line has to deviate or shift in order to cover those, that results in giving the bad output for even the valid inputs(that produces a predicted good outcome).
* The output can be greater than 1 or it can be 0, because there is no squash.

**Therefore we need the best fit line and for that we are using the sigmoid function. Sigmoid function is defined as:**

$$f(x) = \frac{1}{1 + e^{-x}}$$

#### The hyphothesis is defined as:
$$h_\theta(x) = \frac{1}{1 + e^{-\theta^T x}}$$

* if $z \ge 0$ , $g(z) \ge 0.5$
* if $z \le 0$ , $g(z) \le 0.5$

**The curve in Logistic Regression is Non convex because there are multiple local minima and a single global minima. So we Need a cost function function that solves the problem of local minima.**

#### The cost function is defined as:
$$J(\theta) = -\frac{1}{m} \sum_{i=1}^{m} \left[ y^{(i)} \log(h_\theta(x^{(i)})) + (1 - y^{(i)}) \log(1 - h_\theta(x^{(i)})) \right]$$

* **Asymptote for $y=1$:** $\lim_{h_\theta(x) \to 0} -\log(h_\theta(x)) = \infty$
* **Asymptote for $y=0$:** $\lim_{h_\theta(x) \to 1} -\log(1 - h_\theta(x)) = \infty$