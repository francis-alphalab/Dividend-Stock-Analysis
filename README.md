# Dividend Stock Analysis

A Python-based analysis of five high-dividend stocks using historical data
from Yahoo Finance. This project explores dividend yield, total return vs
price-only return, correlation, and portfolio optimization via the
Efficient Frontier.

## Stocks Analyzed
- **KO** — Coca-Cola
- **JNJ** — Johnson & Johnson
- **XOM** — ExxonMobil
- **PG** — Procter & Gamble
- **T** — AT&T

## Project Structure

### 1. Dividend Yield
Bar chart comparing the trailing 12-month dividend yield for each stock.
T has the highest yield at 3.86%, JNJ the lowest at 2.14%.

### 2. Cumulative Performance
Line chart comparing price-only return vs total return (adjusted close)
for each stock from 2015 to present. Highlights the compounding value
of dividends over time.

### 3. Correlation Heatmap
Heatmap of daily return correlations between all 5 stocks using adjusted
close prices. KO and PG show the highest correlation (0.62), while XOM
is the most independent mover.

### 4. Efficient Frontier
Monte Carlo simulation of 10,000 random portfolios. Each portfolio is
plotted by risk vs return and colored by Sharpe ratio. Highlights:
- **Max Sharpe Portfolio** — best risk-adjusted return
- **Minimum Variance Portfolio** — lowest possible risk
- Hover over any point to see the exact stock weights

## Tools Used
- Python
- pandas
- numpy
- yfinance
- Plotly (Graph Objects)

## Key Findings
- Total return significantly outperforms price-only return for all 5 stocks
- XOM has the lowest correlation with other stocks — useful for diversification
- The Max Sharpe portfolio allocates heavily to KO (~46%) given its
strong risk-adjusted performance
- Risk-free rate used: 3.69% (US 3-Month T-Bill, April 2026)
