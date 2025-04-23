# AmityTech
Wellington Hackathon

Overview
Welcome to AmityTech, a cutting-edge project developed during the Wellington Hackathon!
This solution focuses on optimizing delivery routes through reinforcement learning to tackle real-world logistics challenges, especially when priority handling is critical.
We implement a custom delivery environment built with Gymnasium, powered by a Proximal Policy Optimization (PPO) agent from Stable-Baselines3.
Our system is designed to minimize delivery times while dynamically prioritizing high-priority deliveries, ensuring that life-critical and urgent orders are always delivered first.

Key Features:

-Custom Reinforcement Learning Environment: Tailored to simulate realistic delivery conditions, including order urgency, rider movement penalties, and completion rewards.

-Proximal Policy Optimization (PPO): A powerful reinforcement learning algorithm that trains the agent to make smarter decisions over time.

-Priority Handling System: High-priority deliveries are weighted more heavily during training, ensuring the agent learns to prioritize them without manual rule setting.

-Penalty and Reward Shaping:
  -1 penalty per rider move to encourage efficiency.
  +10 reward for successful deliveries.
  Extra weight for high-priority order completions.

Dynamic Decision-Making: The agent adapts routing decisions in real time based on the urgency and location of pending deliveries.

Policy-Based Learning Approach: The model focuses on learning the best action directly from observed states, ensuring fast and adaptive learning curves.

Technologies Used:
-Python 3.11
-Gymnasium
-Stable-Baselines3
-Proximal Policy Optimization
-Numpy / Matplotlib
-PyTorch / TensorFlow

It works by:

  1)Initialize Environment: Simulates multiple delivery requests with a mix of normal and high-priority packages.
  2)Agent Interaction: The agent selects the best moves/actions based on the current environment state.
  3)Reward System: The agent receives rewards for quick, efficient deliveries and penalties for unnecessary moves.
  4)Policy Update: Using PPO, the agent updates its policy to maximize cumulative rewards over episodes.
  5)Prioritization Effect: Over time, the agent naturally learns that high-priority deliveries lead to better outcomes, adjusting strategies to prioritize them without being explicitly told.



