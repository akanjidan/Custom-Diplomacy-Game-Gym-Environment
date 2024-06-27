# Custom-Diplomacy-Game-Gym-Environment

This code contains a custom implementation of a Gym environment for the Diplomacy game, along with testing, validation, and training using Proximal Policy Optimization (PPO).

# Table of Contents
  1.	Installation
  2.	Usage
  3.	Project Structure
  4.	Description of Files
  5.	Custom Diplomacy Gym Class
  6.	Testing the Environment
  7.	Validation
  8.	Training with PPO
  9.	Contributing
  10.	License

      
# Installation
To run this notebook, you need to install the required dependencies. You can install them using the following commands:
pip install diplomacy
pip install gymnasium
pip install "stable-baselines3[extra]>=2.0.0a4"

# Usage
To use this notebook, open it in Jupyter Notebook or JupyterLab and execute the cells in order. The notebook is divided into sections that handle different aspects of creating and testing a custom Gym environment for Diplomacy, as well as training an agent using PPO.

# Project Structure
The notebook contains the following main sections:
1. Imports and Necessary Installations: Installs and imports required libraries.
2. Custom Diplomacy Gym Class: Defines the custom Gym environment for the Diplomacy game.
3. Testing the Environment: Tests the custom environment to ensure it works correctly.
4. Validation: Runs a validation test to demonstrate the environment's functionality.
5. Training with PPO: Trains an agent using the PPO algorithm in the custom environment.

# Custom Diplomacy Gym Class
This section defines the `DiplomacyStrategyEnv` class, a custom implementation of a Gym environment for the Diplomacy game. The class includes methods for initializing the environment, resetting it, stepping through actions, rendering, and closing the environment.
Key Methods
•	__init__(): Initializes the environment.
•	reset(): Resets the environment to the initial state.
•	step(action): Executes an action and returns the next state, reward, done flag, and info.
•	check_max_action(): Check the maximum possible action for the agent.
•	observation_data_to_observation(): creates the observation space for the environment.
•	calculate_reward(previous_state, actions_taken, new_state, our_agent): Calculate the reward at a given time step for the agent.
•	_init_observation_space(): Create the MultiDiscrete space for the observation space.

# Testing the Environment
This section includes code for testing the custom Gym environment to ensure it functions correctly. It uses random actions to interact with the environment and checks for expected behavior.

# Validation
In the validation section, the environment is tested with random actions from the multi-discrete action space. The aim is to validate that the environment runs correctly and the game mechanics are properly implemented.

Training with PPO
This section demonstrates how to train an agent using the Proximal Policy Optimization (PPO) algorithm. The agent is trained to play the Diplomacy game within the custom environment.

Contributing
Contributions are welcome! 

