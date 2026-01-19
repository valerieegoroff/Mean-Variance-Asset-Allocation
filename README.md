# Mean-Variance-Asset-Allocation
Mean–Variance portfolio analysis and asset allocation using historical excess returns, with a focus on diversification, Sharpe ratios, and the role of TIPS.

# Mean-Variance Asset Allocation

Mean–variance portfolio analysis and asset allocation using historical excess returns across multiple asset classes.

## Overview

This project applies mean–variance portfolio theory to analyze and compare different asset allocation strategies using historical monthly excess returns. The focus is on understanding risk-adjusted performance, diversification benefits, and the role of Treasury Inflation-Protected Securities (TIPS) within a multi-asset portfolio.

All returns are excess returns, and all reported performance statistics are annualized.

## Assets Analyzed

The investment universe includes a diversified set of asset classes:
- U.S. equities  
- Domestic bonds  
- Foreign bonds  
- Treasury Inflation-Protected Securities (TIPS)  
- Other diversified asset exposures  

## Methodology

- Computed annualized mean excess return, volatility, and Sharpe ratio for each asset  
- Analyzed the correlation matrix to assess diversification across asset classes  
- Constructed the mean–variance tangency portfolio  
- Compared the ranking of asset Sharpe ratios to optimal portfolio weights  
- Evaluated the role of TIPS through sensitivity analysis:
  - Dropping TIPS from the investment universe  
  - Increasing expected TIPS excess returns relative to historical estimates  
- Built and compared multiple allocation strategies under a targeted return constraint:
  - Equally weighted  
  - Risk-parity (inverse-variance weighted)  
  - Mean–variance optimized  

Each portfolio was rescaled to achieve the same target expected return to allow for a fair comparison across allocation methods.

## Tools Used

- Python  
- pandas  
- NumPy  
- matplotlib  

## Results

The analysis highlights how diversification and correlation structure influence optimal portfolio construction. While mean–variance optimization produces the strongest in-sample risk-adjusted performance, simpler allocation approaches such as equal weighting and risk parity provide more stable and robust portfolios.

The TIPS sensitivity analysis suggests that TIPS can meaningfully impact the efficient frontier, particularly when treated as a distinct asset class rather than grouped with nominal bonds.

## Key Takeaways

- Diversification benefits depend heavily on correlation structure, not just individual asset performance  
- Mean–variance optimization is powerful but sensitive to estimation error  
- Simpler allocation rules can offer greater robustness  
- TIPS may expand the investment opportunity set when modeled separately  
