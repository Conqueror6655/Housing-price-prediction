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

