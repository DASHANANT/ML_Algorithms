
** Linear discriminant analysis (LDA), normal discriminant analysis (NDA), or discriminant function analysis is a generalization of Fisher's linear discriminant,
a method used in statistics and other fields, to find a linear combination of features that characterizes or separates two or more classes of objects or events. 
The resulting combination may be used as a linear classifier, or, more commonly, for dimensionality reduction before later classification. **

-
![image]()

LDA for two classes
Consider a set of observations {\displaystyle {\vec {x}}}{\vec {x}} (also called features, attributes, variables or measurements) for each sample of an object or event with known class {\displaystyle y}y. This set of samples is called the training set. The classification problem is then to find a good predictor for the class {\displaystyle y}y of any sample of the same distribution (not necessarily from the training set) given only an observation {\displaystyle {\vec {x}}}{\vec {x}}.[10]:338

LDA approaches the problem by assuming that the conditional probability density functions {\displaystyle p({\vec {x}}|y=0)}p({\vec {x}}|y=0) and {\displaystyle p({\vec {x}}|y=1)}p({\vec {x}}|y=1) are both normally distributed with mean and covariance parameters {\displaystyle \left({\vec {\mu }}_{0},\Sigma _{0}\right)}\left({\vec {\mu }}_{0},\Sigma _{0}\right) and {\displaystyle \left({\vec {\mu }}_{1},\Sigma _{1}\right)}\left({\vec {\mu }}_{1},\Sigma _{1}\right), respectively. Under this assumption, the Bayes optimal solution is to predict points as being from the second class if the log of the likelihood ratios is bigger than some threshold T, so that:

{\displaystyle ({\vec {x}}-{\vec {\mu }}_{0})^{T}\Sigma _{0}^{-1}({\vec {x}}-{\vec {\mu }}_{0})+\ln |\Sigma _{0}|-({\vec {x}}-{\vec {\mu }}_{1})^{T}\Sigma _{1}^{-1}({\vec {x}}-{\vec {\mu }}_{1})-\ln |\Sigma _{1}|\ >\ T}({\vec {x}}-{\vec {\mu }}_{0})^{T}\Sigma _{0}^{-1}({\vec {x}}-{\vec {\mu }}_{0})+\ln |\Sigma _{0}|-({\vec {x}}-{\vec {\mu }}_{1})^{T}\Sigma _{1}^{-1}({\vec {x}}-{\vec {\mu }}_{1})-\ln |\Sigma _{1}|\ >\ T
Without any further assumptions, the resulting classifier is referred to as QDA (quadratic discriminant analysis).

LDA instead makes the additional simplifying homoscedasticity assumption (i.e. that the class covariances are identical, so {\displaystyle \Sigma _{0}=\Sigma _{1}=\Sigma }\Sigma _{0}=\Sigma _{1}=\Sigma ) and that the covariances have full rank. In this case, several terms cancel:

{\displaystyle {\vec {x}}^{T}\Sigma _{0}^{-1}{\vec {x}}={\vec {x}}^{T}\Sigma _{1}^{-1}{\vec {x}}}{\vec {x}}^{T}\Sigma _{0}^{-1}{\vec {x}}={\vec {x}}^{T}\Sigma _{1}^{-1}{\vec {x}}
{\displaystyle {\vec {x}}^{T}{\Sigma _{i}}^{-1}{\vec {\mu }}_{i}={{\vec {\mu }}_{i}}^{T}{\Sigma _{i}}^{-1}{\vec {x}}}{\displaystyle {\vec {x}}^{T}{\Sigma _{i}}^{-1}{\vec {\mu }}_{i}={{\vec {\mu }}_{i}}^{T}{\Sigma _{i}}^{-1}{\vec {x}}} because {\displaystyle \Sigma _{i}}\Sigma _{i} is Hermitian
and the above decision criterion becomes a threshold on the dot product

{\displaystyle {\vec {w}}\cdot {\vec {x}}>c}{\vec {w}}\cdot {\vec {x}}>c
for some threshold constant c, where

{\displaystyle {\vec {w}}=\Sigma ^{-1}({\vec {\mu }}_{1}-{\vec {\mu }}_{0})}{\vec {w}}=\Sigma ^{-1}({\vec {\mu }}_{1}-{\vec {\mu }}_{0})
{\displaystyle c={\vec {w}}\cdot {\frac {1}{2}}({\vec {\mu }}_{1}+{\vec {\mu }}_{0})}{\displaystyle c={\vec {w}}\cdot {\frac {1}{2}}({\vec {\mu }}_{1}+{\vec {\mu }}_{0})}
This means that the criterion of an input {\displaystyle {\vec {x}}}{\displaystyle {\vec {x}}} being in a class {\displaystyle y}y is purely a function of this linear combination of the known observations.

It is often useful to see this conclusion in geometrical terms: the criterion of an input {\displaystyle {\vec {x}}}{\displaystyle {\vec {x}}} being in a class {\displaystyle y}y is purely a function of projection of multidimensional-space point {\displaystyle {\vec {x}}}{\displaystyle {\vec {x}}} onto vector {\displaystyle {\vec {w}}}{\displaystyle {\vec {w}}} (thus, we only consider its direction). In other words, the observation belongs to {\displaystyle y}y if corresponding {\displaystyle {\vec {x}}}{\displaystyle {\vec {x}}} is located on a certain side of a hyperplane perpendicular to {\displaystyle {\vec {w}}}{\displaystyle {\vec {w}}}.
The location of the plane is defined by the threshold c.
