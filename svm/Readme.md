
SVM - Support vector machine
A support vector machine (SVM) is a supervised machine learning model that uses classification algorithms for two-group classification problems.


- How Does SVM Work?
- support-vector machine constructs a hyperplane or set of hyperplanes in a high- or infinite-dimensional space, which can be used for classification, regression, or other tasks like outliers detection.[3] Intuitively, a good separation is achieved by the hyperplane that has the largest distance to the nearest training-data point of any class (so-called functional margin), since in general the larger the margin, the lower the generalization error of the classifier

![Kernel_Machine.svg](https://en.wikipedia.org/wiki/File:Kernel_Machine.svg)

To keep the computational load reasonable, the mappings used by SVM schemes are designed to ensure that dot products of pairs of input data vectors may be computed easily in terms of the variables in the original space, by defining them in terms of a kernel function {\displaystyle k(x,y)}{\displaystyle k(x,y)} selected to suit the problem.[6] The hyperplanes in the higher-dimensional space are defined as the set of points whose dot product with a vector in that space is constant, where such a set of vectors is an orthogonal (and thus minimal) set of vectors that defines a hyperplane. The vectors defining the hyperplanes can be chosen to be linear combinations with parameters {\displaystyle \alpha _{i}}\alpha _{i} of images of feature vectors {\displaystyle x_{i}}x_{i} that occur in the data base. With this choice of a hyperplane, the points {\displaystyle x}x in the feature space that are mapped into the hyperplane are defined by the relation {\displaystyle \textstyle \sum _{i}\alpha _{i}k(x_{i},x)={\text{constant}}.}{\displaystyle \textstyle \sum _{i}\alpha _{i}k(x_{i},x)={\text{constant}}.}

Note that if {\displaystyle k(x,y)}{\displaystyle k(x,y)} becomes small as {\displaystyle y}y grows further away from {\displaystyle x}x, each term in the sum measures the degree of closeness of the test point {\displaystyle x}x to the corresponding data base point {\displaystyle x_{i}}x_{i}. In this way, the sum of kernels above can be used to measure the relative nearness of each test point to the data points originating in one or the other of the sets to be discriminated.
