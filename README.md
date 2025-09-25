

1️⃣ What assumptions does linear regression make?
Linear regression relies on several key assumptions:
Linearity: The relationship between independent and dependent variables is linear.
Independence: Observations are independent of each other.
Homoscedasticity: Constant variance of errors across all levels of the independent variables.
Normality of errors: Residuals (errors) are normally distributed.
No multicollinearity: Independent variables are not highly correlated with each other.

Violating these can lead to biased or inefficient estimates.

2️⃣ How do you interpret the coefficients?
Each coefficient represents the expected change in the dependent variable for a one-unit increase in the corresponding independent variable, holding all other variables constant.

For example, if the coefficient for `bedrooms` is 500, it means adding one bedroom increases the predicted price by ₹500 (assuming price is the target).



3️⃣ What is R² score and its significance?
R² (Coefficient of Determination) measures how well the model explains the variability of the target variable.
 Ranges from 0 to 1
 0 → model explains none of the variability.
 1 → model explains all the variability.
 A higher R² means a better fit, but beware of overfitting in complex models.


 4️⃣ When would you prefer MSE over MAE?
MSE (Mean Squared Error) penalizes larger errors more heavily (due to squaring), making it useful when large errors are especially undesirable.
MAE (Mean Absolute Error) treats all errors equally and is more robust to outliers.
MSE when you want to emphasize large deviations and MAE when you want a balanced view of average error**.

 5️⃣ How do you detect multicollinearity?
Variance Inflation Factor (VIF): A VIF > 5 or 10 indicates high multicollinearity.
Correlation matrix: Look for high correlations between independent variables.
Unstable coefficients: If small changes in data cause large swings in coefficients, multicollinearity might be present.


 6️⃣ What is the difference between simple and multiple regression?
| Type               | Description                                      |
|--------------------|--------------------------------------------------|
| Simple Regression | One independent variable    |
| Multiple Regression | Two or more independent variables |

Simple regression is easier to visualize, but multiple regression captures more complex relationships.


7️⃣ Can linear regression be used for classification?
no  linear regression is designed for continuous outputs. However: It’s sometimes misused for binary classification (e.g., predicting 0/1), but this leads to poor probability calibration.
Logistic regression is the proper tool for classification tasks.


 8️⃣ What happens if you violate regression assumptions?
Linearity violation → model misses patterns.
Heteroscedasticity → inefficient estimates, unreliable confidence intervals.
Non-normal errors → invalid hypothesis tests.
Multicollinearity → unstable coefficients, hard to interpret.
Autocorrelation→ biased standard errors, especially in time series.

