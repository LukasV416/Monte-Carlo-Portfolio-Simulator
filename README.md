# Monte-Carlo-Portfolio-Simulator
This project uses Monte Carlo Simulations as well as Geometric Brownian Motion to model portfolio returns. It incorporates Value-at-Risk (VaR), and percentile based performance metrics using historical stock data from yfinance.

**Key Features:**
  - Pulls historical stock data via yfinance.
  - Allows for customizable equity portfolios.
  - Simulates 10,000 future portfolio outcomes using GBM.
  - Calculates performance metrics incluiding expected portfolio value, 95% and 99% VaR, and the 25th, 50th, and 75th percentile outcomes.
  - Generates a histogram of simulated final portfolio values.

**How It Works:**
1. **Download Historical Prices**
   - Automatically fetches closing prices for the selected tickers (default: AAPL, AMZN, MSFT, TSLA) over the past 3 years.
  
2. **Compute Daily Returns**
   - Converts price data into daily percentage returns and applies user defined portfolio weights.
  
3. **Simulates Portfolio Growth**
   - Simulates Geometric Brownian Motion to model portfolio growth 10,000 times.
  
4. **Evaluate Results**
   - Produces statistical metrics and a histogram of simulated final portfolio values.
  
