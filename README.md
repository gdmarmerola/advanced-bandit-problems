# advanced-bandit-problems

## Implementing harder bandit problems and their solutions

Extending my [first repository about reinforcement learning](https://github.com/gdmarmerola/interactive-intro-rl), I will post here tutorials on Jupyter Notebooks on how to solve harder bandit problems, focusing on cases that have few practical implementations on the community and current research. 

## Available tutorials

Following is a small description of the available bandit tutorials in this repository.

### Non-stationary bandits

In non-stationary bandits, the distribution of true expected rewards for each bandit changes over time. In the tutorial, we present two scenarios: (a) true expected rewards changes suddenly and (b) true expected rewards changes slowly and linearly. We show results for two policies: the epsilon-greedy policy and Thompson Sampling. Our results point to TS superiority, being quicker to adapt to new conditions and exploring more efficiently. We also show an anlysis on buffer size for TS, showing how to balance continuous exploration (smaller buffer size and more adaptability) with exploitation (larger buffer sizes with less adaptability).

### Approximate bayesian inference for bandits

In this tutorial, we tackle the Multi-armed bandit problem with Gaussian rewards by using approximate bayesian inference techniques to compute the posterior distribution over expected rewards for each arm. We present exact inference (through a conjugate Normal prior), MCMC Sampling (Metropolis-Hastings algorithm), Variational Inference (Black box VI) and Bootstrapping and compare their results on the Gaussian MAB. We show implementations from scratch and using `edward`.

### Risk-aware bandits

In this Notebook, we explore a Gaussian bandit setting where the reward distributions have different risks. We define a new reward function, the Conditional Value-at-Risk (CVaR) so we can make decisions based on a risk appetite parameter. We test and compare Thompson Sampling, Bayesian UCB, and the MaRaB algorithm. In large simulations, TS showed the best results, with MaRaB being very competitive at low-risk scenarios.

Hope these tutorials help people looking for a hands-on approach to bandits. I will post more stuff in the future!
