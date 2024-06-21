# Chaos-Playground-Pursuit-Evasion
# Pursuit-Evasion Game in a Reinforcement Learning Setting

## Overview
This project models a pursuit-evasion game in a discrete 20x20 grid using reinforcement learning.

## Implementation Strategies
1. **Mean Field Method**: 
   - In this implementation, all the pursuers know the actions (not positions) of the other pursuers which are within a certain radius of that pursuer.
   - Each pursuer uses these actions of some the other pursuers to create a an effective Mean Field agent according to the Mean Field Theory
   - Highly scalable for a large number of agents.
2. **Full State Approach**:
   - All pursuers knows the positions of all the other pursuers. 
   - Accompanied with curse of dimensionality, hence not very scalable.
## Training Method
- **Deep Q-Network (DQN)**: 
  - Trains agents using Q-learning to optimize their strategies.
## Results
- The full state approach achieves a slightly better average pursuer reward compared to the mean field method.
- The mean field method offers better scalability for larger agent populations.

