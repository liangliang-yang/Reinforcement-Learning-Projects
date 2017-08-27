# rldm-project-2

The purpose of this project report is to build a learning agent to successfully land the "Lunar Lander" that is implemented in OpenAI gym. We will use the LunarLander-v2 gym environment, where the agent need to navigate a space vehicle from the starting point to the landing pad on the surface of moon without crashing. 
Recall the problem in last homework (HW4), which is a reinforcement learning problem with discrete state and action spaces, we can solve it with simple Q-learning method. However, the task in the project is a problem with a continuous state space (so our state space is infinite). We can't use any table to store infinite number of values. In order to solve this problem, here we will use a recent version of Q-learning called Deep Q Network learning (DQN), which can approximate the Q function with a neural network.

In order to improve my model, I applied the Double Learning technique to my full DQN agent, which can help my agent perform more stable and faster. Later I have explored the effect of those hyper-parameters (including alpha, gamma, epsilon). 

The code is included here as myDQN.py, and in order to run the code, you will need to install some additional libraries. The command for this is:

```{python}
pip install theano keras gym
```
For the operating system, I used Ubuntu 16.04 in my virtual box. I have tried install these libraries in my main windows 7 system, but it doesn't work.

The main theroy and implementation of my agent is detailed discussed in the blog "Let’s make a DQN" by Jaromír Janisch. I have referenced his work in the report as well as here. (His blog is very easy to understand).

I have made the youtube video for presentation and the link is as below:
* link: https://www.youtube.com/watch?v=N2TJxbcSGSI&feature=youtu.be

Also for all the related OpenAI experiment link, below is a full list: 
* Full DQN: https://gym.openai.com/evaluations/eval_OVMEjFipS1yM35l9eWKcA
* Double Learning improved Full DQN: https://gym.openai.com/evaluations/eval_eRvOfSTATkWlx9Yb71yqSQ
* Effect of exploration rate (epsilon = exp(- #episode)): https://gym.openai.com/evaluations/eval_vWRKAtS2mNSIiV0Dgwg
* Effect of learning rate (Adam lr = 0.0005): https://gym.openai.com/evaluations/eval_ISIKVa8YRpqdowJAF4HWOQ
* Effect of learning rate (Adam lr = 0.005): https://gym.openai.com/evaluations/eval_ZeiS8I1R1rbd70jxo6A
* Effect of gamma (discount factor gamma = 0.5): https://gym.openai.com/evaluations/eval_VwVeBJbQuugvvR4fPAWA


### Reference:

[Let’s make a DQN, Jaromír Janisch](https://jaromiru.com/2016/09/27/lets-make-a-dqn-theory/)
