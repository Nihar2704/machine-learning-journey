## Cost Fucntion

### Mean Squared Error(MSE) 

 $$MSE = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2$$

 #### Advantages
 * It is Differentiable
 * It has only one local minima and global minima
 
#### Disadvantages

* Not Robust to Outliers
* It changes the unit of output variable

### Mean Absolute Error(MAE)
$$MAE = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i|$$

#### Advantages
* It is robust to outliers
* Does not change the unit of output variable

#### Disadvantages 
* Convergence takes time
* Optimization process is complex

### Root Mean Squared Error(RMSE)

$$RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2}$$

#### Advantages 
* Penalizes large error more heavily
* Same unit as the target variable
* Differentiable function
* Widely accepted and easy to compare

#### Disadvantages
* Very sensitive to ouliers
* Not Robust for noisy data
* Computationally more expensive than MAE
* Harder to explain than MAE

