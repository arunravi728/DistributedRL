# DistributedRL

This project is my first foray into developing AI infrastucture for AI training. The aim is to build a minimal by functional distributed reinforcement learning (RL) training pipeline. Focussing on RL agents allows me to draw on my prior experience training RL models as part of my work with [BadgerRL](https://github.com/Badger-RL).

#### Goals
- Trains multiple agents in parallel across nodes (using separate processes or machines).
- Profiles and reduces network latency and communication overhead.
- Monitors and optimizes GPU utilization across the distributed environment.
- Collects metrics (like reward convergence, episode throughput, bandwidth usage).
- Optionally supports environments like OpenAI Gym or PettingZoo (for multi-agent cases).

#### Step 1: Single Node Baseline RL Agent
The first step would be to locally train RL agents on a single node/machine. I will compare the performance between on-policy and off-policy algorithms on environments with discrete and continuous action spaces.

###### Algorithms - 
1. PPO - On-Policy
2. TD3 - Off-Policy

###### Environments - 
1. [CartPole](https://gymnasium.farama.org/environments/classic_control/cart_pole/) - Discrete Action Space
2. [CarRacing](https://gymnasium.farama.org/environments/box2d/car_racing/) - Continuous Action Space

