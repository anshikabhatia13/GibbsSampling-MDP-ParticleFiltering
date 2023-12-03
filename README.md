# AI Algorithms Implementation

This repository contains Python implementations of several AI algorithms that I developed as part of the AI course at IIT Ropar. The implemented algorithms include:

1. Gibbs Sampling
2. Particle Filtering for Robot Localization
3. Markov Decision Process Algorithm

## Contents

- [Gibbs Sampling](#gibbs-sampling)
- [Particle Filtering](#particle-filtering)
- [Markov Decision Process Algorithm](#markov-decision-process-algorithm)
- [Usage](#usage)
- [Acknowledgments](#acknowledgments)

## Gibbs Sampling

Gibbs Sampling is a Monte Carlo algorithm for obtaining a sequence of observations from a multivariate probability distribution.
![Particle Filtering Example](/images/particle_filtering_example.png)


### Implementation Details

The Gibbs Sampling implementation  in this repository follows these key steps:

1. **Initialization**: Initialize the state of each variable in the Bayesian network randomly or based on some initial conditions.

2. **Sequential Sampling**: Iterate through each variable in the network, updating its value based on the values of the other variables. This is done sequentially, one variable at a time.

3. **Conditional Distributions**: At each iteration, sample the value of the current variable conditioned on the values of the other variables. This step involves using the conditional probability distribution of the variable given its neighbors in the network.

4. **Repeat**: Repeat the sequential sampling process for a sufficient number of iterations to allow the algorithm to converge to the true distribution.

## Particle Filtering

Particle Filtering is an approximate inference method used for probabilistic inference over complex Dynamic Bayesian Networks (DBNs).
![Particle Filtering Example](/images/particle_filtering_example.png)


### Implementation Details

The Particle Filtering implementation  in this repository follows these key steps:

1. **Initialization**: Generate an initial population of particles (samples) representing possible states of the system. Each particle includes a set of variables that characterize the state.

2. **Transition Model**: Move each particle to the next state based on a transition model, capturing the temporal evolution of the system.

3. **Observation Weighting**: Assign weights to particles based on how well they match the observed evidence or measurements. This step involves comparing the predicted observations of each particle with the actual observations.

4. **Resampling**: Create a new population of particles by randomly sampling from the current particles, with the probability of selection proportional to their weights. This step helps focus the particles on regions of higher likelihood.

5. **Repeat**: Iterate through the steps of transition, observation weighting, and resampling to track the system's state over time.


## Markov Decision Process Algorithm

The Markov Decision Process (MDP) algorithm is used for decision-making in situations where the outcome is uncertain.
![Particle Filtering Example](/images/particle_filtering_example.png)


### Implementation Details


The MDP algorithm implementation  in this repository follows these key steps:

1. **State and Action Space**: Define the state space representing possible states of the system and the action space representing possible actions that can be taken.

2. **Transition Model**: Specify the transition probabilities, indicating the likelihood of transitioning from one state to another after taking a particular action.

3. **Reward Model**: Define the rewards associated with each state-action pair, representing the immediate benefit or cost of taking a particular action in a specific state.

4. **Policy Iteration or Value Iteration**: Implement either policy iteration or value iteration to find the optimal policy, which determines the best action to take in each state to maximize the expected cumulative reward.

5. **Usage of the Optimal Policy**: Once the optimal policy is obtained, it can be used for decision-making in the given environment.


## Usage

To use any of the implemented algorithms, open the .ipynb file in Google Colaboratory and run.


