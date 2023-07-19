# Linear Regression
Linear Regression with regularisations and cross-validation code from scratch!

This analysis involves applying linear regression with regularization techniques. The dataset used for this analysis can be accessed at the following open-source website: http://cogsys.imm.dtu.dk/propulsionmodelling/data.html.

The initial code provided a basic approach to data cleaning. Since the dataset contains a limited number of variables, no feature ranking procedures have been performed (refer to my other project for feature ranking using ensemble methods like XGBoost and Random Forest).

In order to gain a comprehensive understanding of the dataset, several plots are presented, including the correlation matrix. However, it is important to note that relying solely on the correlation matrix to assess the impact of predictors on the target variable for linear regression is not recommended due to potential linear dependencies among the features.

The code provides a test set which is 25% of the whole dataset. The validation and training set together are the remaining 75% of the whole dataset.
Then a linear regression function is written with many features; regularizations can be selected: 
  1. Normalizing features can be turned on
  2. Lasso, Ridge, or the default one which is the least squares 
  3. Certain plots can be turned on for a qualitative understanding of the predictions
  4. Certain error quantities can be computed for a quantitative understanding of the predictions.

