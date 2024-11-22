# Different Machine Learning Methods on Classification Problem
在这个项目里面，我们将使用监督学习，非监督学习（SVM）,强化学习（深度Q学习和演员评论家算法），用于NSL KDD数据集上进行分类问题，并到探索其的优缺点。

The NSL-KDD dataset consists of network traffic data collected from a simulated computer network environment. The network traffic includes both normal and various types of attack activities. The dataset provides a diverse range of intrusion scenarios, making it suitable for evaluating the performance of intrusion detection systems.

In this study, we used the pre-processed and normalized NSL-KDD dataset as the environment. The columns (features) of the NSL-KDD dataset were used as the states for the DQN. The dataset contains a total of 42 features, and we used the first 41 features as states. The 42nd feature is the label used for computing the reward vector based on model predictions [2]. 

![Table 1: List of features on NSL-KDD dataset](description.png "Optional Title")

总的来说，这些方法在nsl-kdd上均可以得到较多的TP和TN,以及较少对的FP,但是均有较大的FN. 目前的epoch测试在500-1000左右。目前的改进方法在于是否提升hidden network的数量和layer的层数，以及epoch是否够，因为nsl_kdd数据库有40多个attrubute.

总体来说。几个模型的结果接近。Accuracy和F1大体为0.78-0.82， 召回率为0.68-0.72， 精确度则高达0.93-0.95，这表明在模型预测为阳性的数据中，实际是阳性的正确率较高，然而模型还是存在漏掉真正阳性将其判断成阴性，还需要按照上面说的几点进行改正

1. 非监督学习方法
我们就用的最简单的SVM method。
最后得出在test data上面的结果如下
![Table 2: Confusion Matrix for SVM](result_SVM/20241118_215457/confusion_matrix.png "Optional Title")

2. 监督学习方法
![Table 3: Confusion Matrix for SL](result_SL\20241119_110824\confusion_matrix.png "Optional Title")
