# 1. Introduction
## A. Elements:
* policy : the learning agent’s way of behaving at a given time
* reward signal : 
    * the goal in a reinforcement learning problem
    * goal: maximize the total reward it receives over the long run
* value function: the total amount of reward an agent can expect to accumulate over the future, starting from that state.
* Environment: a model of the environment

## B. Compare with supervised/unsupervised learning
* Supervised Learning: RL do not have a labeled dataset, it explores the best policy by itself. 
* Unsupervised Learning: RL try to find the best policies to interact with the environment, UL try to find the unstructured information from the data. 

## C. Limitation:
* The evolution algorithm: estimate the directions
the parameters should be adjusted in order to most rapidly improve a policy's performance
* optimization is not the same an optimality

# 2. Tabular Solution Methods
## A. Cover:
* all the core ideas of reinforcement learning algorithms in their simplest forms
* solution methods for the special of the reinforcement learning problem in which there is only a single state, called bandit problems
* finite Markov decision processes

## B. n-Armed Bandit Problem
* Your objective is to maximize the expected total reward over some time period
* Greedy action : exploiting your current knowledge of the values of the actions

## C. Action- Value Method:
* Estimated value: $Q_t(a) = \frac{R_1 + \cdots + R_{N_t(a)}} {N_t(a)}$
    * $N_t(a) = 0$ choose default value for Q
    * $N_t(a) -> \inf$ approximating real value
* $\$