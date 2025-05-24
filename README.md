
# Portfolio Optimization Using Python

**Name:** Kavini Hasanga Gamalath  

##  Project Overview

This project applies **Modern Portfolio Theory (MPT)** using Python to construct and analyze an optimal investment portfolio. It includes:
- Historical data collection via `yfinance`
- Risk and return metric calculations
- Monte Carlo simulation to visualize the Efficient Frontier
- Optimization using `scipy.optimize` to maximize the Sharpe Ratio and minimize risk

---

##  Features & Tasks

###  Task 1: Data Collection & Preprocessing
- Collected 5 years of daily adjusted close prices for 5 S&P 500 companies using `yfinance`
- Cleaned missing values and computed daily returns

###  Task 2: Expected Returns & Risk Calculation
- Calculated annualized mean returns and covariance matrix
- Simulated a random portfolio to calculate expected return and risk

###  Task 3: Monte Carlo Simulation
- Simulated 10,000 random portfolios
- Visualized the Efficient Frontier with Sharpe Ratios

###  Task 4: Portfolio Optimization
- Used `scipy.optimize.minimize` to:
  - Maximize Sharpe Ratio
  - Minimize Portfolio Variance
- Plotted optimized portfolios on the efficient frontier

###  Task 5: Analysis & Reporting
- Interpreted results and portfolio suitability for investor types
- Explained methodology and challenges overcome

---

##  Setup Instructions

### Dependencies
Ensure you have Python 3.7+ and install the following packages:

```bash
pip install yfinance numpy pandas matplotlib scipy
```

###  Files to Run

- **`portfolio_optimization.ipynb`**: Main Jupyter Notebook containing code and visualizations.

---

##  How to Run

1. Clone or download the project folder.
2. Open the notebook using Jupyter:
   ```bash
   jupyter notebook portfolio_optimization.ipynb
   ```
3. Run all cells from top to bottom.

---

##  Architecture & Logic Flow

```text
1. Load Libraries & Select Stocks
2. Download Data using yfinance
3. Calculate Daily Returns
4. Compute Annualized Returns & Covariance
5. Simulate 10,000 Portfolios (Monte Carlo)
6. Optimize Portfolio using scipy.optimize
7. Visualize Efficient Frontier
8. Analyze Results for Investor Suitability
```

---

##  Portfolio Summary

| Portfolio           | Expected Return | Volatility | Sharpe Ratio |
|---------------------|------------------|------------|---------------|
| Max Sharpe Ratio    | 26.53%           | 24.72%     | 0.99          |
| Min Variance        | 8.93%            | 15.10%     | 0.46          |

---

###  Technical Architecture
- **Language**: Python 3
- **Libraries**: `yfinance`, `numpy`, `pandas`, `matplotlib`, `scipy.optimize`
- **Approach**: Modern Portfolio Theory using real-time market data

###  Challenges Faced
- Handling missing data and time alignment
- Understanding Sharpe Ratio optimization logic
- Fine-tuning simulation visuals (color mapping and readability)
- Getting optimization constraints right using `SLSQP`

###  How I Overcame Them
- Used `.dropna()` to clean data
- Broke down the Sharpe ratio formula into helper functions
- Used color gradients and alpha blending in `matplotlib`
- Carefully read `scipy.optimize` documentation and used lambda constraints

---

##  References

1. Python for Finance: Portfolio Optimization – https://blog.mlq.ai/python-for-finance-portfolio-optimization/
2. yfinance Documentation – https://pypi.org/project/yfinance/
3. SciPy Optimize – https://docs.scipy.org/doc/scipy/reference/optimize.html
4. NumPy & Pandas Docs – https://numpy.org/ | https://pandas.pydata.org
5. Matplotlib – https://matplotlib.org

---


