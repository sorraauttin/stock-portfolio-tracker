# Stock Portfolio Tracker
**Portfolio Project 3 | Python + yfinance**

A live stock portfolio tracker that fetches real-time prices from Yahoo Finance, calculates profit and loss for each holding, and generates price history and portfolio breakdown charts.

---

## What This Project Does

- Reads your portfolio from a simple CSV file (ticker, shares, buy price)
- Fetches the **live current price** of each stock from Yahoo Finance
- Calculates cost basis, current value, gain/loss (฿ and %) for every holding
- Generates a **1-year price history chart** per stock (green = profit, red = loss)
- Generates a **portfolio breakdown pie chart** showing allocation by value

---

## Sample Portfolio

| Ticker | Company | Market |
|--------|---------|--------|
| TSM | Taiwan Semiconductor | NYSE (US) |
| GOOG | Alphabet (Google) | NASDAQ (US) |
| DELTA.BK | Delta Electronics Thailand | SET (TH) |
| MINT.BK | Minor International | SET (TH) |
| VT | Vanguard Total World ETF | NYSE (US) |

> Thai SET stocks require the `.BK` suffix (e.g., `DELTA.BK`). US stocks use plain tickers.

---

## Tools Used

| Tool | Purpose |
|------|---------|
| Python (pandas, matplotlib) | Data processing and charting |
| yfinance | Live stock price API |
| Jupyter Notebook | Analysis environment |

---

## How to Run

```bash
pip install yfinance pandas matplotlib
jupyter notebook stock_tracker.ipynb
```

To track different stocks, edit `portfolio.csv` — no code changes needed.

---

## Output

| File | Description |
|------|-------------|
| `Price_history.png` | 1-year price chart for each holding |
| `Portfolio_value.png` | Pie chart of portfolio allocation by current value |
