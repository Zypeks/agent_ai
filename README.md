
# Stock Trading with Reinforcement Learning

This repository contains two Jupyter Notebooks that demonstrate the use of reinforcement learning algorithms to trade stocks. The algorithms implemented are Proximal Policy Optimization (PPO) and Deep Q-Network (DQN). These notebooks utilize historical stock data and reinforcement learning techniques to create trading agents that can make buy or sell decisions based on predefined indicators and market conditions.

## Notebooks

### 1. PPO_z_score_indeksy.ipynb
This notebook implements a trading strategy using the Proximal Policy Optimization (PPO) algorithm. It includes the following steps:
- **Data Loading:** Historical stock data for several companies (e.g., Intel, IBM, Nvidia) is loaded.
- **Environment Setup:** A custom trading environment is created using the `gym-anytrading` package, with features such as RSI and SMA indicators.
- **Training the PPO Agent:** The PPO algorithm is used to train the agent on the given stock data.
- **Evaluation:** The performance of the trained agent is evaluated and visualized.

### 2. DQN_z_score_indeksy.ipynb
This notebook implements a trading strategy using the Deep Q-Network (DQN) algorithm. The structure of this notebook is similar to the PPO notebook:
- **Data Loading:** The same stock data is used.
- **Environment Setup:** The environment is prepared in a way compatible with the DQN algorithm.
- **Training the DQN Agent:** The DQN algorithm is used to train the trading agent.
- **Evaluation:** The agent's performance is analyzed and compared to the PPO approach.

## Requirements

To run the notebooks, you need to have the following Python packages installed:

- `pandas`
- `numpy`
- `matplotlib`
- `gym`
- `gym-anytrading`
- `stable-baselines3`
- `talib`
- `torch`

You can install these dependencies using pip:

```bash
pip install pandas numpy matplotlib gym gym-anytrading stable-baselines3 ta-lib torch
```

## Running the Notebooks

1. Clone the repository:

```bash
git clone https://github.com/yourusername/stock-trading-rl.git
cd stock-trading-rl
```

2. Launch Jupyter Notebook:

```bash
jupyter notebook
```

3. Open the desired notebook (`PPO_z_score_indeksy.ipynb` or `DQN_z_score_indeksy.ipynb`) and run the cells sequentially.

## Results

The notebooks include visualizations and statistics that demonstrate the performance of the PPO and DQN agents in simulated stock trading scenarios. These include profit/loss analysis, total rewards, and trade actions (buy/sell points).

## License

This project is licensed under the MIT License.
