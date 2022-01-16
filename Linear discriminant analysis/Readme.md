# Linear Discriminant Analysis
----------------------------
Linear Discriminant Analysis or Normal Discriminant Analysis or Discriminant Function Analysis is a dimensionality reduction technique that is commonly used for supervised classification problems. It is used for modelling differences in groups i.e. separating two or more classes. It is used to project the features in higher dimension space into a lower dimension space. 

Two criteria are used by LDA to create a new axis: 

Maximize the distance between means of the two classes.
Minimize the variation within each class.

 
Extensions to LDA: 
------------

- Quadratic Discriminant Analysis (QDA): Each class uses its own estimate of variance (or covariance when there are multiple input variables).
- Flexible Discriminant Analysis (FDA): Where non-linear combinations of inputs are used such as splines.
- Regularized Discriminant Analysis (RDA): Introduces regularization into the estimate of the variance (actually covariance), moderating the influence of different variables on LDA.


![image](https://github.com/DASHANANT/ML_Algorithms/blob/main/Linear%20discriminant%20analysis/lda_1.png)


