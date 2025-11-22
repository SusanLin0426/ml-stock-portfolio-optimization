# ml-stock-portfolio-optimization
This project applies ML models—regression, Random Forest, SVR, and XGBoost—to predict stock price movements and build optimal portfolios. Using fundamental, technical, and sentiment data from Taiwanese firms, we compare model accuracy, simulated returns, and risk control.

### Project Overview
This project applies machine learning to forecast stock price trends and construct an optimal investment portfolio. We evaluate multiple models—including Regression, RandomForest, XGBoost, and SVR—measure performance, simulate investment outcomes, and provide data-driven portfolio recommendations.
- Investment period: March–May 2023
-  Initial capital: NT$100,000
-  Trading rule: Only one buy and one sell action allowed

### Data Sources
Fundamental Data
- TEJ Financial Database (historical prices, balance sheets, income statements, cash flow statements)

Technical Data
- Yahoo Finance
- Goodinfo! Taiwan Stock Information
- TWSE

### Research Framework
1. Industry & Company Selection
- 5 industries × 2 companies each (10 total)

2. Data Cleaning & Feature Engineering
- Financial statement preprocessing
- Missing value handling
- Technical indicator calculation (KD, RSI, MACD, moving averages)
- Time-series train/test splitting
- Feature correlation filtering & multicollinearity removal

3. Model Training
- Fundamental models: Regression, XGBoost, SVR
- Technical models: RandomForest, SVR, XGBoost
- Hyperparameter tuning
- Forecasting June 2023 stock prices (fundamental)
- Forecasting next 60 trading days (technical)

4. Portfolio Construction
- Select stocks with positive predicted returns
- Allocate weights based on forecasted price movement
- Calculate expected capital allocation and shares purchased

5. Simulation & Model Comparison
- Evaluate actual return as of June 2, 2023
- Compute overall return and annualized return
