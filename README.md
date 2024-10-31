# Reinforcement-learning
CIA-1 AND CIA-2

StockOptimizerUCB Class: Upper Confidence Bound (UCB) Stock Optimization
------------------------------------------------------------------------
The StockOptimizerUCB class optimizes stock selection over multiple actions using the Upper Confidence Bound (UCB) algorithm, balancing exploration and exploitation to maximize rewards. It simulates stock and comparison views and calculates rewards based on differences. In each time step, it selects an action based on UCB values, updates Q-values based on rewards received, and records them in a history array. The results are visualized with a heatmap showing Q-value evolution over time and a bar plot displaying average Q-values, helping to highlight the most effective actions.

Key Methods:
------------
get_reward: Computes reward by simulating viewer counts.
select_action: Chooses actions using UCB values.
update_estimates: Updates Q-values with received rewards.
plot_results: Visualizes Q-values via heatmap and bar plot.


QLearningAgent Class: Q-Learning for Grid Environment Navigation
-----------------------------------------------------------------
The QLearningAgent class is a reinforcement learning agent trained via Q-learning to navigate a grid environment, with rewards for reaching a goal and penalties for obstacles. It initializes a Q-table to store state-action values and uses epsilon-greedy policy to balance exploration (random actions) and exploitation (optimal actions). During each episode, the agent selects actions, updates Q-values with temporal difference updates, and iterates until reaching the goal.

Key Methods:
------------
choose_action: Chooses actions based on epsilon-greedy policy.
update: Updates Q-values using Q-learning updates.
train: Runs the agent through multiple episodes to refine Q-values.
Simulation
The main function initializes a 10x10 grid environment with obstacles, trains the agent, and visualizes the learned Q-values in a heatmap, revealing optimal paths and decision points for the agent.

