 # Naive Bayes classifier
-------------------------------------------------------------------------------------------
 Theorem with an assumption of independence among predictors. In simple terms, a Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature.

For example, a fruit may be considered to be an apple if it is red, round, and about 3 inches in diameter. Even if these features depend on each other or upon the existence of the other features, all of these properties independently contribute to the probability that this fruit is an apple and that is why it is known as ‘Naive’.

Naive Bayes model is easy to build and particularly useful for very large data sets. Along with simplicity, Naive Bayes is known to outperform even highly sophisticated classification methods.

Bayes theorem provides a way of calculating posterior probability P(c|x) from P(c), P(x) and P(x|c).
Look at the equation below:


-------------------------------------------------------------------------------------------
![img](https://www.analyticsvidhya.com/wp-content/uploads/2015/09/Bayes_rule-300x172.png)


# How Naive Bayes algorithm works?
-------------------------------------------------------------------------------------------
  Let’s follow the below steps to perform it.

- Step 1: Convert the data set into a frequency table
- Step 2: Create Likelihood table by finding the probabilities 
- Step 3: Now, use Naive Bayesian equation to calculate the posterior probability for each class. 
        The class with the highest posterior probability is the outcome of prediction.
        
 

Why naive Bayes called Naive?
-------------------------------
Beacuse it assumes conditional independence of features
