## what is machine learning?
Is a science of programming systems that can learn from data.

churn detetion
computer vision
score credict
retail decisions

## how to fix underfiting in machine learning?
- get better features (using feature engineering)
- reduce constraints(hyperparameters) for example regularization param

### error rate is called OOS (out of sample error)

# End to end Machine Learning System

## Look at the Big Picture

##### 1. Define the objetive in business terms
- The goal of the company is to achive accurate prediction of housing prices by district.
- Determinate whether it is worth investing in a given area.
- Maximize revenue which is directly affected by the 2 goals mentioned above.

##### 2. How will your solution be used?
- The model's output will serve as input for another machine learning system, which determinate wheter it is worth invest in the area.

##### 3. What are the current solutions/workaraounds?
- A team of experts collets up to date data about a district and determinates the median housing price, but when they are unable to obtain accurate data, they estimate the price housing using complex formulas.

##### 4. How would you frame this problem (supervised/unsupervised, online/offline, etc)?
- *Type of learning:* Supervised learning (we already know the expected output)
- *Algorithm / task:* Regression (multiple regression - multiple features) (univariate regression - predict a single value)
- *Learning technique:* Batch learning
##### 5. How performance should be measured?
- Using RMSE (root mean square error), it measure how much error the system makes in its predictions. RMSE uses $l_{2}$ norm *(euclidean distance, used in Ridge normalization).*\
  
$$
RMSE(\bold{X}, h) =\sqrt{\frac{1}{m}\sum_{i=1}^{m}(h(\bold{x}^{(i)}) -y^{(i)})^{2}}
$$
where:
    - $m$ is the number of instances in the dataset.
    - $\bold{x}$ is a vector of all the feature values.
    - $y$ is the desired output.
    - $\bold{X}$ is a matrix containing all the feature values.
    - $h$ is the hypothesis, in other words the predicted value as well knows as $\hat{y}$

- If there are many predicted $\hat{y}$ outliers, you may consider using MAE mean absolute error, it uses $l_1 norm$ (manhattan distance, used in lasso norm).\
$$MAE(\bold{X}, h) = \frac{1}{m} \sum_{i=1}^{m} \left|h(\bold{x}^{(i)}) - y^{(i)}\right|$$
##### 6.
#####
#####
#####
