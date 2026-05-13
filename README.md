# comp569_ArtificialIntelligence
Sustainable Agriculture and Resource Management
# Sustainable Agriculture AI (MDP + Reinforcement Learning)

## 📌 Project Overview

This project implements an AI system for **Sustainable Agriculture and Resource Management** using:

* Markov Decision Processes (MDPs)
* Value Iteration
* Policy Iteration
* Q-Learning (Reinforcement Learning)

The goal is to optimize long-term farming decisions such as irrigation, fertilization, harvesting, and conservation under uncertainty.

---

## 🧠 Problem Description

Agricultural systems involve uncertainty in:

* Weather conditions
* Soil moisture
* Crop growth
* Resource availability

This project models agriculture as a **108-state Markov Decision Process** to compute optimal decision-making policies.

---

## ⚙️ Technologies

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📂 Project Structure

```id="7zq8n4"
project_3_SARM.ipynb   # Full implementation (MDP + RL + experiments)
README.md              # Documentation
```

---

## 🚀 How to Run

### 1. Clone Repository

```id="g7nq2x"
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies

```id="c5y0tw"
pip install numpy pandas matplotlib seaborn
```

### 3. Run Notebook

```id="5h7m2a"
jupyter notebook project_3_SARM.ipynb
```

---

## ▶️ Implementation Details

### State Space

* 108 total states
* Variables:

  * Soil moisture (Dry, Moderate, Wet)
  * Crop stage (4 stages)
  * Nutrient level (3 levels)
  * Water availability (3 levels)

### Actions

* Irrigate
* Fertilize
* Harvest
* Conserve

---

## 🤖 Algorithms Implemented

### 1. Value Iteration

* Converged in **205 iterations**
* Final Bellman error: **0.000953**
* Mean state value: **641.36**

### 2. Policy Iteration

* Converged in **7 iterations**
* 100% policy agreement with Value Iteration

### 3. Q-Learning

* Trained for **5000 episodes**
* Final reward (last 100 episodes): **~129**
* Policy agreement with optimal: **36.1%**

---

## 📊 Results Summary

### Policy Evaluation (100 Episodes)

| Algorithm        | Mean Reward | Success Rate |
| ---------------- | ----------- | ------------ |
| Value Iteration  | 145.04      | 100%         |
| Policy Iteration | 145.07      | 100%         |
| Q-Learning       | 141.86      | 100%         |

---

## 📈 Key Insights

* Value Iteration and Policy Iteration produce identical optimal policies
* Policy Iteration converges much faster
* Q-Learning learns effective behavior but does not fully match optimal policy
* Decay-based exploration strategies improve reinforcement learning performance
* Reward design strongly influences system behavior

---

## 🧪 Experiments Conducted

* Discount factor (γ) analysis
* Learning rate (α) tuning
* Exploration strategies (fixed vs decay)
* Reward function (harvest reward) analysis

---

## 🔍 Example Behavior

* Dry soil → Irrigate
* Low nutrients → Fertilize
* Mature crops → Harvest
* Adequate conditions → Conserve

---

## 🔮 Future Work

* Use real-world agricultural data
* Expand state space
* Apply Deep Reinforcement Learning (DQN)
* Incorporate weather prediction models

---

## 👤 Author

Arya Singh

---

## 📘 Course

COMP 569 – Artificial Intelligence
California State University Channel Islands
