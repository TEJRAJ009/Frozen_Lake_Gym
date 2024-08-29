# Reinforcement Learning with Q-learning on FrozenLake ❄️ 

This project demonstrates the implementation of **Q-learning**, a popular reinforcement learning algorithm, on the **FrozenLake** environment provided by OpenAI Gym. The goal is to help an agent learn an optimal policy to navigate a frozen lake and reach a goal without falling into holes.

## Overview

In this project, I:
- Implemented Q-learning from scratch.
- Tuned hyperparameters such as learning rate, discount factor, and exploration rate.
- Trained an agent to solve the FrozenLake environment.
- Evaluated the performance of the trained agent.

## Environment

**FrozenLake** is a grid world where an agent must move from a start state to a goal state on a grid of frozen tiles. Some tiles are slippery (holes), and if the agent steps on them, it falls into the water and the episode ends.

## Key Concepts

### Q-learning

Q-learning is a model-free reinforcement learning algorithm that seeks to learn the value of a given action in a particular state. The algorithm updates its Q-values based on the Bellman equation:

![image](https://github.com/user-attachments/assets/6fde6f92-a0b7-4921-819a-16f52d7135c5)


Where:
- \(s\) is the current state
- \(a\) is the action taken
- \(r\) is the reward received
- \(s'\) is the next state
- \(\alpha\) is the learning rate
- \(\gamma\) is the discount factor

### Hyperparameters

- **Learning Rate (\(\alpha\))**: Controls how much the Q-values are updated each time.
- **Discount Factor (\(\gamma\))**: Determines the importance of future rewards.
- **Exploration Rate (\(\epsilon\))**: Controls the trade-off between exploration and exploitation.

## How to Run

### Running on Google Colab

This project can be run on **Google Colab**, which provides free access to GPUs and TPUs, making it suitable for those who don't have access to powerful local machines.

1. Open the notebook in Google Colab by clicking the "Open in Colab" badge above.
2. Run all cells to start training the Q-learning agent.
3. Follow the instructions in the notebook to visualize the training process and the results.

### Running Locally (It's a Pain if you Have Windows)

To run this project locally, you need to have Python and the required libraries installed.

1. **Clone this repository**:
    \`\`\`bash
    git clone [https://github.com/your-username/reinforcement-learning-frozenlake.git](https://github.com/TEJRAJ009/Frozen_Lake_Gym.git)
    cd reinforcement-learning-frozenlake
    \`\`\`

2. **Install dependencies**:
    \`\`\`bash
    pip install apt install xvfb
    pip install gym[atari]
    pip install gym-notebook-wrapper
    pip install atari-py
    \`\`\`

3. **Run the Jupyter Notebook**:
    \`\`\`bash
    jupyter notebook Reinforcement_with_OpenAI_Gym.ipynb
    \`\`\`

## Results

After training, the agent should be able to navigate the FrozenLake environment with a high success rate. The notebook provides visualizations of the training process and the final policy learned by the agent.

## Contributions

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue if you find a bug or have a feature request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- OpenAI Gym for providing the FrozenLake environment.
- Google Colab for enabling cloud-based computation.
"""
