# multiple-linear-regression
I have build a model by using multiple linear regression , backward elimination technique. by using backward elimination technique we can only optimal independent variable which is highly statistically significant and has great impact on the dependent variable profit.
A very simple python program to implement Multiple Linear Regression using the LinearRegression class from sklearn.linear_model library.

The program uses the statsmodels.formula.api library to get the P values of the independent variables. The variables with P values greater than the significant value ( which was set to 0.05 ) are removed. The process is continued till variables with the lowest P values are selected are fitted into the regressor ( the new dataset of independent variables are called X_Optimal ).

X_Optimal is again split into training set and test set using the test_train_split function from sklearn.model_selection.

The regressor is fitted with the X_Optimal_Train and Y_Train variables and the prediction for Y_Test ( the dependent varibale) is done using the regressor.predict(X_Optimal_Test)
