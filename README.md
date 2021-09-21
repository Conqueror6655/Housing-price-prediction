# Housing-price-prediction
Using simple models we have to predict housing price based on the property columns given

# Overview :-
Housing is one of the necessities of human life, and demand is increasing day by day. It is now essential to predict house prices as accurately as possible. The price is dependent on various factors while predicting. House prediction is useful for not only buyers and sellers but also helps in maintaining the economy of the region. The main aim of this project is to predict the sale prices of residential houses in Ames, Iowa. For achieving our purpose, we are using the dataset provided on Kaggle for training and testing purposes.

From the above Evaluation scores and Output Plots, we can observe that we are getting the best results in boosting algorithms. We are getting worst results in Lasso Regression. From the figures, we can see that all the boosting regressors are testing the model well and predicting the proper results as compared to regularisations.

The accuracy can be increased by using neural networks and doing some more preprocessing

Some brief description about the models used:-

# Linear Regression :-
Linear Regression is the fundamental and old technique for predicting quan- titative values, but it is still a practical approach. In linear regression, it assumes that there is a linear relationship between the output Y and input
X. In our case, Y is the target price, and it assumes that it will be having the linear relationship between all the features acting as X. Mathematically, we can denote it as:

Y ≈ β0 + β1 ∗ X1 + ... + β1 ∗ XN
Where Y is output and X1 to XN are the N input features and it uses the given data to estimate the values of β’s. They are selected to minimize the sum of squared residuals. We fit the straight line that best fits in our training sample and predict the values based on the fitted line. We applied linear regression for our model as the first regression model.

# Ridge Regression and Lasso Regression :-
Next, we have evaluated our results on the ridge and lasso regression. Both of these regressions are similar to least squares, but for minimizing the β coefficients, a different mathematical concept used.
For Ridge:
  Google the formula can't type in this file

where λ is tuning parameter and the second λ term is known as shrinkage penalty. The tuning parameter λ used to adjust the relative effect of two terms on the coefficient of regression.

 
For Lasso:
   Google the formula can't type in this file
 
Lasso regression is similar to the ridge but overcomes the disadvantage of Ridge Regression. Ridge regression will reduce the magnitude of coefficients, but it will never exclude any parameter, but it is possible with lasso regres- sion. We have trained our model with both ridge and lasso. By comparing with all the mentioned regression model, we can observe in our evaluation part that we are getting good results in lasso, then slightly lower results with ridge then slightly lower with linear because of the mentioned reasons. There are a few disadvantages of Lasso regression also. Like sometimes in case of more than one highly correlated variable, it will select one and ignore the others. To overcome these, we have ElasticNet, Google the formula can't type here.

It is having a unique minimum because of quadratic term that’s make the strongly convex loss function. We can observe a better results than lasso in this while training our model.

# Boosting:
For the comparisons, we have tried to train our model with also boosting to see the results. Boosting algorithms is an ensemble technique to convert weak learners to keen learners. Gradient Boosting do not change the weight Gradient Boosting do not change the weight of every incorrect regressor, but it will try to t the new predictor to the remaining error by the last predictors. XGBoost means eXtreme Gradient Boosting. Traditional Gradient boosting works in the sequential pattern, so it is slow. LightGBM and XGBoost both are an advancement of Gradient Boosting with high speed. We have used all these three models to train our model and calculated the r2 and RMSE.

