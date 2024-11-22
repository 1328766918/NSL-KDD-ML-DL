# Different Machine Learning Methods on Classification Problem
在这个项目里面，我们将使用监督学习，非监督学习（SVM）,强化学习（深度Q学习和演员评论家算法），用于NSL KDD数据集上进行分类问题，并到探索其的优缺点。

The NSL-KDD dataset consists of network traffic data collected from a simulated computer network environment. The network traffic includes both normal and various types of attack activities. The dataset provides a diverse range of intrusion scenarios, making it suitable for evaluating the performance of intrusion detection systems.

In this study, we used the pre-processed and normalized NSL-KDD dataset as the environment. The columns (features) of the NSL-KDD dataset were used as the states for the DQN. The dataset contains a total of 42 features, and we used the first 41 features as states. The 42nd feature is the label used for computing the reward vector based on model predictions [2]. 

![Table 1: List of features on NSL-KDD dataset](description.png "Optional Title")

1. 非监督学习方法
我们就用的最简单的SVM method。
最后得出在test data上面的结果如下

