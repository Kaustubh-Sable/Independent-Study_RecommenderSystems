For getting familiarized with Reinforcement Learning, I will be going through the Hello World program of Reinforcement Learning - **Multi-Armed Bandit Problem**

#### Problem Formulation
* Slot machine with n arms.
* Stochastic reward of either R=+1 for success, or R=0 for failure

#### Objective:
To pull the arms one-by-one in sequence such that we maximize our total reward collected in the long run.

![Multi-Armed Bandit Problem](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Reinforcement_Learning/Images/MultiArm_Bandit.png)

Non-triviality of the multi-armed bandit problem lies in the fact that we (the agent) cannot access the true bandit probability distributions — all learning is carried out via the means of trial-and-error and value estimation.

##### Our Strategy: Epsilon-greedy agent
With a probability ϵ, we will choose an action a at random, 
and 
the rest of the time (probability 1−ϵ) we will choose the best lever based on what we currently know from past plays.

##### Action-value function:
![Example](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Reinforcement_Learning/Images/ActionValue_function.png)

Above definition can be re-written recursively as:
![Example](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Reinforcement_Learning/Images/ActionValue_REW.png)

Greedily choose an action from our Q(a):
![Example](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Reinforcement_Learning/Images/GreedyAction.png)

#### Example:
![Example](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Reinforcement_Learning/Images/Example.png)

#### Notes
* More information on NDCG and word2Vec can be found in this [presentation](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Slides/KS_Week8_Reco_Sys.pptx).
* The python notebook can also be seen live on *Google Colab* here: https://colab.research.google.com/drive/1OudhokrWzhHjlyWmbtBRgc9AwZQBcAEj?usp=sharing

#### References
* Reinforcement Learning - Multi-Armed Bandit problem: https://towardsdatascience.com/solving-the-multi-armed-bandit-problem-b72de40db97c 
* Code for the Multi-Armed Bandit Problem: https://github.com/ankonzoid/LearningX/tree/master/classical_RL/multiarmed_bandit 
