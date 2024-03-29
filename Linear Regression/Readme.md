# Linear Regression
----------------------------------------------------------------------------------------
![](https://github.com/DASHANANT/ML_Algorithms/blob/main/Linear%20Regression/linear%20regression.png)

# Normal Equations 
---------------------------------------------------------------------------------------
The closed-form solution should be preferred for "smaller" datasets where calculating (a "costly") matrix inverse is not a concern. For very large datasets, or datasets where the inverse of [XTX] may not exist (the matrix is non-invertible or singular, e.g., in case of perfect multicollinearity), the QR, SVD or gradient descent approaches are to be preferred.

The linear function (linear regression model) is defined as:
--------------------------------------------------------------------------------------------
y= w0x0 + w1x1 +...+ wmxm = ∑i= wT.x
----------------------------------------------------------------------------------------------
where y is the response variable, x is an m-dimensional sample vector, and w is the weight vector (vector of coefficients). Note that w0 represents the y-axis intercept of the model and therefore x0=1.

Using the closed-form solution (normal equation), we compute the weights of the model as follows:

W=(xT .x)^-1.xT. y
--------------------------------------------------------------------------------------------------
