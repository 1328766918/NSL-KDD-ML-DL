NSL-KDD Dataset
The NSL-KDD dataset consists of network traffic data collected from a simulated computer network environment. The network traffic includes both normal and various types of attack activities. The dataset provides a diverse range of intrusion scenarios, making it suitable for evaluating the performance of intrusion detection systems.

In this study, we used the pre-processed and normalized NSL-KDD dataset as the environment [1]. The columns (features) of the NSL-KDD dataset were used as the states for the DQN. The dataset contains a total of 42 features, and we used the first 41 features as states. The 42nd feature is the label used for computing the reward vector based on model predictions [2].

![Table 1: List of features on NSL-KDD dataset](https://example.com/path/to/111.png "Optional Title")
