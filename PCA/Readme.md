-- WHAT IS PRINCIPAL COMPONENT ANALYSIS?
- Principal Component Analysis, or PCA, is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets, 
by transforming a large set of variables into a smaller one that still contains most of the information in the large set.

- Reducing the number of variables of a data set naturally comes at the expense of accuracy, but the trick in dimensionality 
reduction is to trade a little accuracy for simplicity. Because smaller data sets are easier to explore and visualize and
make analyzing data much easier and faster for machine learning algorithms without extraneous variables to process.

STEP BY STEP EXPLANATION OF PCA
- STEP 1: STANDARDIZATION
- ![form](https://builtin.com/sites/default/files/styles/ckeditor_optimize/public/inline-images/Principal%20Component%20Analysis%20Standardization.png)

- STEP 2: COVARIANCE MATRIX COMPUTATION
- ![form1](https://builtin.com/sites/default/files/styles/ckeditor_optimize/public/inline-images/Principal%20Component%20Analysis%20Covariance%20Matrix.png)

- STEP 3: COMPUTE THE EIGENVECTORS AND EIGENVALUES OF THE COVARIANCE MATRIX TO IDENTIFY THE PRINCIPAL COMPONENTS

- ![gif](https://builtin.com/sites/default/files/inline-images/Principal%20Component%20Analysis%20second%20principal.gif)

- STEP 4: FEATURE VECTOR
to choose whether to keep all these components or discard those of lesser significance (of low eigenvalues),
and form with the remaining ones a matrix of vectors that we call Feature vector.


- STEP 5: RECAST THE DATA ALONG THE PRINCIPAL COMPONENTS AXES

- ![last](https://builtin.com/sites/default/files/styles/ckeditor_optimize/public/inline-images/Principal%20Component%20Analysis%20feature%20vector.png)
