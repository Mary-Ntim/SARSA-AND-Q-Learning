# 🧠 GridWorld RL Assignment: SARSA vs. Q-learning

This repository contains the full implementation and analysis of SARSA and Q-learning algorithms applied to a 5x5 GridWorld navigation task. The goal is to compare how both agents learn optimal policies using ε-greedy action selection and evaluate their performance through trajectory plots and episode reward trends.

---

## 📌 Task Summary

- **Environment**: 5x5 GridWorld
- **Start state**: 21 (bottom-left)
- **Terminal states**: 1 and 5 (top-left and top-right)
- **Penalty zones**: States 16, 17, 19, 20 → −20 reward and reset to start
- **Regular move**: −1 reward per step
- **Goal**: Learn the optimal path to a terminal while minimizing penalties

The agent uses **ε-greedy exploration** and learns with both:
- **SARSA** (on-policy)
- **Q-learning** (off-policy)

---

## 🗂️ Repository Structure

```bash
.
├── gridworld.py             # Environment definition
├── sarsa.py                 # SARSA training and evaluation
├── q_learning.py            # Q-learning training and evaluation
├── plot_trajectory.py       # Grid and trajectory plot generator
├── reward_plot.py           # Reward trend visualization
├── README.md                # This file
└── results/
    ├── sarsa_trajectory.png
    ├── q_learning_trajectory.png
    └── reward_plot.png

pip install numpy matplotlib

