# rldm-project-3

The purpose of this project report is try to replicate several multi-agent Q learning algorithms that learn equilibrium policies described in the Greenwald (2003) paper.  We will focus on the "soccer game" described in the paper, which is a zero-sum two-player Markov game with no deterministic equilibrium policies. The four algorithms we will mainly discussed in this report is normal Q, Friend-Q, Foe-Q and Correlated-Q, and also there will be four figures shown below. The goal is to gain a better understanding of how these algorithms work in detail.

For the 4 experiments, I used python for coding and testing. In particular, I write the code and run in IPython of jupyter notebook. You will find there are totally six py files. Four of them are related to different Q learner that are discussed in the paper. The other two, one is used to setup the environment for the soccer game, and the other one is used to run the experiment and visualize the result.

The running/testing of the code is very simple. Just open a python shell and copy/paste the code in the first part and run all the necessary functions. Typically, for the Foe_Q and Correlated_Q, since I use the solvers.lp() function, we will need to install the CVXOPT package.

Also the youtube video presentation link is:

https://youtu.be/4HhKpojXews


### Reference: 

*   http://cvxopt.org/examples/tutorial/lp.html?highlight=linear

*  https://pdfs.semanticscholar.org/7480/4472b338283a5b92659db76b55f9eaef8b74.pdf

* http://jmlr.csail.mit.edu/papers/volume4/hu03a/hu03a.pdf



