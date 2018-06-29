# advanced-bandit-problems

## Implementing harder bandit problems and their solutions

Extending my [first repository about reinforcement learning](https://github.com/gdmarmerola/interactive-intro-rl), I will post here tutorials on Jupyter Notebooks on how to solve harder bandit problems, focusing on cases that have few practical implementations on the community and current research. 

## Available tutorials

Following is a small description of the available bandit tutorials in this repository.

### Non-stationary bandits

In non-stationary bandits, the distribution of true expected rewards for each bandit changes over time. In the tutorial, we present two scenarios: (a) true expected rewards changes suddenly and (b) true expected rewards changes slowly and linearly. We show results for two policies: the epsilon-greedy policy and Thompson Sampling. Our results point to TS superiority, being quicker to adapt to new conditions and exploring more efficiently. We also show an anlysis on buffer size for TS, showing how to balance continuous exploration (smaller buffer size and more adaptability) with exploitation (larger buffer sizes with less adaptability).

Hope these tutorials help people looking for a hands-on approach to bandits. I will post more stuff in the future!
