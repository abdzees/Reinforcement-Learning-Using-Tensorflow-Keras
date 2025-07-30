# Deep Q-Learning with Keras-RL2 on CartPole-v1 using Gymnasium

This project demonstrates how to train a Deep Q-Network (DQN) agent to solve the classic CartPole-v1 environment using **Keras-RL2**, **TensorFlow 2.10**, and **Gymnasium**.

## Overview

- **Environment:** CartPole-v1 from Gymnasium, wrapped to be compatible with Keras-RL2.
- **Agent:** Deep Q-Network (DQN) with a neural network function approximator.
- **Model Architecture:**  
  A simple feedforward neural network with two hidden layers (24 neurons each, ReLU activations) that predicts Q-values for each action.
- **Training:**  
  The agent is trained for 50,000 steps to learn how to balance the pole by maximizing cumulative rewards.
- **Testing:**  
  After training, the agent is tested for multiple episodes with environment rendering enabled to visualize the learned behavior.
- **Saving/Loading:**  
  The trained model weights are saved and can be reloaded for further testing or deployment.

## Key Features

- Uses the latest **Gymnasium** environment with the correct `render_mode='human'` for visualization.
- Implements a custom environment wrapper to adapt Gymnasium's API to Keras-RL2's expected format.
- Utilizes a Boltzmann policy for action selection to balance exploration and exploitation.
- Compatible with TensorFlow 2.10 and Keras-RL2 for reinforcement learning tasks.
- Visualization support during testing to observe the agent's performance in real-time.

## Dependencies

- tensorflow==2.10  
- keras-rl2  
- gymnasium  
- pygame  
- numpy

## Usage

1. Install dependencies (use the provided versions for compatibility).  
2. Run the training script to train the DQN agent.  
3. Test the trained agent and observe the CartPole balancing visually.  
4. Save and load model weights for persistence.

## During Training
![CartPole Balancing Preview](cartpole_preview.gif)

---

This project serves as a foundation for understanding and experimenting with deep reinforcement learning on classic control problems using modern libraries.
