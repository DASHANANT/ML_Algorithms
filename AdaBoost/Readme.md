# AdaBoost 

AdaBoost, short for Adaptive Boosting, is a statistical classification meta-algorithm.
It can be used in conjunction with many other types of learning algorithms to improve performance. 
The output of the other learning algorithms ('weak learners') is combined into a weighted sum that represents the final output of the boosted classifier. 

AdaBoost is adaptive in the sense that subsequent weak learners are tweaked in favor of those instances misclassified by previous classifiers. In some problems it can be less susceptible to the overfitting problem than other learning algorithms. 

The individual learners can be weak, but as long as the performance of each one is slightly better than random guessing, the final model can be proven to converge to a strong learner.Every learning algorithm tends to suit some problem types better than others, and typically has many different parameters and configurations to adjust before it achieves optimal performance on a dataset.

AdaBoost (with decision trees as the weak learners) is often referred to as the best out-of-the-box classifier. When used with decision tree learning, information gathered at each stage of the AdaBoost algorithm about the relative 'hardness' of each training sample is fed into the tree growing algorithm such that later trees tend to focus on harder-to-classify examples.

--------------------------------------------
![](https://th.bing.com/th/id/OIP.QXRQ26gT3ZkyY0EvKFHDUAHaEv?pid=ImgDet&rs=1)
![](https://th.bing.com/th/id/R.417450dba813dd993263412f2851c350?rik=xj1kTjRMZX23eA&riu=http%3a%2f%2faa.ssdi.di.fct.unl.pt%2fLectures%2flec%2fimg%2fL12-stumping.gif&ehk=Ei8RUC6nvphBBvLs5rw1%2bdeKftF6nwquPMn0x6lmTUI%3d&risl=&pid=ImgRaw&r=0)
