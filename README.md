# Dueling-Networks-for-Deep-Reinforcement-Learning
This project aims to implement the Dueling Network architecture for Deep Reinforcement Learning and evaluate its performance across multiple environments. The environments chosen are CartPole-v1, LunarLander-v3, and Pong-v5 (Atari Game). An Vanilla Deep Q-Network is used as baseline and is compared with the Dueling Deep Q-Network variant of the same model in each environment.

## Code
- The code used to implement and train both baseline DQN and Dueling DQN is present in the `Notebooks` directory.
- A `requirements.txt` file is also present which contains the dependencies which must be installed before running the notebooks.
- The standard nomenclature followed for notebooks is `{architecture}_{environment}`. For example, the notebook `dueling_dqn_lunar_lander` contains code to train and run the Dueling DQN on the LunarLander environment.
- Notebooks which have the suffix `noops` are those whose environments have been modified to contain additional actions which are essentially 'do nothing'. This is done to compare how well the dueling network adapts to a larger and more redundant action space.

## Theory and Results
The results obtained after rigorous experimentation can be observed in multiple ways:
- **Presentation** : The file `Dueling Networks Overview and Results.pdf` provides a brief theoretical background, experimental setup, results, and observations in the project.
- **GIFs** : After training is complete, 3 episodes are run to observe the agent in the particular environment. This folder contains GIFs as visualisations of each episode.
- **Plots** : This directory contains plots corresponding to episode rewards during training. These plots are also discussed in the presentation.