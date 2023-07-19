# Linear Regression with Regularisations and Cross-Validation and Hyperparameter Tuning from Scratch!
Linear Regression with regularisations and cross-validation code from scratch!

This analysis involves applying linear regression with regularization techniques. The dataset used for this analysis can be accessed at the following open-source website: http://cogsys.imm.dtu.dk/propulsionmodelling/data.html.

The initial code provided a basic approach to data cleaning. Since the dataset contains a limited number of variables, no feature ranking procedures have been performed (refer to my other project for feature ranking using ensemble methods like XGBoost and Random Forest).

In order to gain a comprehensive understanding of the dataset, several plots are presented, including the correlation matrix. However, it is important to note that relying solely on the correlation matrix to assess the impact of predictors on the target variable for linear regression is not recommended due to potential linear dependencies among the features.

The code provides a test set which is 25% of the whole dataset. The validation and training set together are the remaining 75% of the whole dataset.
Then a linear regression function is written with many features (not parameters!):
  1. Normalizing features can be turned on
  2. Lasso, Ridge, or the default one which is the least squares 
  3. Certain plots can be turned on for a qualitative understanding of the predictions
  4. Certain error quantities can be computed for a quantitative understanding of the predictions.
  5. Values for hyperparameters can be given

Accordingly, a k-fold cross-validation (CV) function is written in order to improve the predictions and tune the hyperparameters through grid research. The latter one will be explained later.
As a rule of thumb, the number of folds is selected at 10, but it is not a fixed variable. Therefore it is a parameter of the cv function. For certain applications, 5 or 3 folds may be enough.


Consequently, a grid search approach is employed to tune the hyperparameters. This is done through the wirtten k-fold cross-validation function. In this grid search...
