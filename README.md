
# Portfolio Optimization with CAPM and Efficient Frontier

This project focuses on portfolio optimization using historical stock data. It utilizes the Capital Asset Pricing Model (CAPM) and Efficient Frontier analysis to determine optimal asset weights to maximize returns relative to risk. Key financial metrics such as Sharpe Ratio, portfolio returns, and volatility are used to evaluate portfolio performance.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Portfolio Optimization](#portfolio-optimization)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)

## Overview
The main goal of this project is to:
1. Calculate individual stock betas.
2. Estimate expected returns using CAPM.
3. Optimize portfolio weights to maximize the Sharpe Ratio.
4. Visualize the Efficient Frontier for different asset allocations.

## Installation
### Prerequisites
- Python 3.7+
- Required packages:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `yfinance`
  - `scipy`

Install the required packages using pip:
```bash
pip install numpy pandas matplotlib yfinance scipy
```

## Usage
1. **Load and Preprocess Data**:
   - Define the stock tickers and retrieve historical price data.
   - Calculate daily returns and extract individual asset returns and market returns.

2. **Calculate Stock Betas**:
   - Compute each asset's beta based on covariance with the market.

3. **Expected Returns using CAPM**:
   - Calculate expected returns for each asset using CAPM.

4. **Optimize Portfolio**:
   - Optimize weights to maximize the Sharpe Ratio.

5. **Visualization**:
   - Plot the Efficient Frontier with a scatter plot of Sharpe Ratios.

### Running the Notebook
1. Load the stock data:
    ```python
    tickers = ['KR','AEP','DIS','MET','CSCO','SRE','RTX','TMUS','EXEL','GE','GEV','GEN']
    ```

2. Compute asset betas:
    ```python
    betas = {} 
    for stock in asset_returns.columns: 
        ...
    ```

3. Calculate expected returns and optimize portfolio:
    ```python
    optimal_portfolio = optimize_portfolio(mean_returns, cov_matrix)
    ```

4. Visualize Efficient Frontier:
    ```python
    plt.scatter(results[0,:], results[1,:], c=results[2,:], cmap='viridis')
    plt.show()
    ```

## Portfolio Optimization
- **Stock Betas**: Beta values provide a measure of an asset's risk in relation to the market.
