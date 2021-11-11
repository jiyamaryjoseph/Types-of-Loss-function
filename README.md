# Types-of-Loss-function

### ‘Loss’ helps us to understand how much the predicted value differ from actual value
###  Function used to calculate the loss is called as “Loss function”
#### cost function and loss function are synonymous and used interchangeably but they are “different”. A loss function/error function is for a single training example/input. A cost function, on the other hand, is the average loss over the entire training dataset.
### The optimization strategies aim at “minimizing the cost function”.


 ##### Regression Loss Function
 ###### Regression Loss is used when we are predicting continuous values like the price of a house or sales of a company. 
1.   Mean Squared Error: 
        It is the mean of squared differences between the actual and predicted value. If the difference is large the model will penalize it as we are computing the squared difference.
   adv: 1. This is in the form of qudratic equation.(when we plot quadratic eqution we get gradient descend with only globalminima.we dnot get any localminima.)
        2. MSE loss penalizes the model for making large error by squring them.
   disadv: 1.This loss not robust to outliers.
2.  Mean Squared Logarithmic Error Loss:
        Suppose we want to reduce the difference between the actual and predicted variable we can take the natural logarithm of the predicted variable then take the mean squared error. This will overcome the problem possessed by the Mean Square Error Method. The model will now penalize less in comparison to the earlier method.

3.   Mean Absolute Error Loss:
        Sometimes there may be some data points which far away from rest of the points i.e outliers, in case of cases Mean Absolute Error Loss will be appropriate to use as it calculates the average of the absolute difference between the actual and predicted values.
   adv. 1. MAE is robust to outliers as compaired to MSE.
   disadv.1.computation is very difficult.bz we are using mode of operand.(I I)
          2.It may have local minima.
  
4.    Huber Loss:
        This is the combination of  Mean Squared Error and Mean Absolute Error Loss.
        
##### Binary Classification Loss Function
###### Suppose we are dealing with a Yes/No situation like “a person has diabetes or not”, in this kind of scenario Binary Classification Loss Function is used.

1.   Binary Cross Entropy Loss:
         It gives the probability value between 0 and 1 for a classification task. Cross-Entropy calculates the average difference between the predicted and actual probabilities.i.e. loss=-ylogy-(1-y)log(1-y).
         -ylog(1-y) if y=0;
         -(1-y)log(1-y) if y=1.
         ('y_predict' is depends on sigmoid function.)
         
##### Multi-Class Classification Loss Function
###### If we take a dataset like Iris where we need to predict the three-class labels: Setosa, Versicolor and Virginia, in such cases where the target variable has more than two classes Multi-Class Classification Loss function is used.
1.    

1.    Cross Entropy:

