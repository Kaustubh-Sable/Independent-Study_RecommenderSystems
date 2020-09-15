Under this topic, I broadly explored the reinforcement learning algorithms used for online advertising in Recommender Systems.

##### Reference
For this study, I mainly studied two research papers. 

#### First paper:
Deep Reinforcement Learning for Online Advertising in Recommender Systems: https://arxiv.org/pdf/1909.03602.pdf 

![Deep Reinforcement Learning for Online Advertising in Recommender Systems](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Online_Advertising/Images/Paper1.png)

##### What does this paper propose?
Creates a Deep-Q Network (DQN) that can determine following three tasks:
* whether to interpolate an ad or not in the recommendation list
* and if yes, the optimal ad and
* the optimal location to interpolate.

Training is based on users’ offline log, which records the interaction history between behavior policy (the advertising strategy in use) and users’ feedback.

###### Autoencoder Based Recommendation
AE is an unsupervised model attempting to reconstruct its input data in the output layer. In general, the bottleneck layer is used as a salient feature representation of the input data. 

Almost all of its variants (denoting AE, variational AE, connective AE, and marginalized AE) can be applied to the recommendation task.

AE can be used to learn the lower-dimensional feature representations at the bottleneck layer.

#### Second paper:
Collaborative Deep Ranking: https://github.com/USCDataScience/Image-Similarity-Deep-Ranking/blob/master/deep_ranking.pdf 

Collaborative Deep Ranking is devised specifically in a pairwise framework for the top-n recommendation. The paper shows that the pairwise model is more suitable for ranking lists generation.

![Collaborative Deep Ranking](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Online_Advertising/Images/Paper2.png)

##### What does this paper propose?
Deep ranking model that employs deep learning technique to learn similarity metric directly from images.
An efficient triplet sampling algorithm is proposed to learn the model.
Simple evaluation metric.
