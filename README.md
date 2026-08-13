
# Ford-GM-Tesla-Stock-Performance-Dashboard

Interactive dashboard analyzing daily stock performance for Ford, GM, and Tesla — comparing returns, volatility, trading volume, and risk across two legacy automakers and one EV disruptor.

##  Project Overview

This project analyzes daily OHLCV (Open, High, Low, Close, Volume) stock data for **Ford**, **General Motors**, and **Tesla** from **January 2021 to February 2022**, and turns it into an interactive dashboard for comparing performance across the three companies.

The dashboard provides insight into total return, daily volatility, trading volume, price swings, and how closely the three stocks move together.

The main goal of this project is to turn raw daily price data into a clear read on **which stock performed best, which carried the most risk, and how the two legacy automakers compare to the EV leader** over the same window.

##  Project Objective

The objective of this project is to:

- Compare total return performance across Ford, GM, and Tesla
- Track cumulative return month by month
- Measure volatility (risk) for each stock
- Identify each stock's best and worst single trading day
- Compare total trading volume across the three companies
- Test how correlated the three stocks are with each other
- Turn the findings into a clear investment-style narrative

## 📊 Key Performance Indicators

| KPI | Value |
|---|---|
| 📅 Trading Days Analyzed | 290 |
| 📦 Total Shares Traded (all 3 combined) | 38.2B |
| 🏆 Best Total Return | Ford, +109.3% |
| 📉 Avg. Daily Volatility (Std Dev) | 2.97% |

## 🔍 Key Insights

### 🏁 Total Return
- **Ford was the standout performer**, up **+109.3%** over the period — more than 6x GM's return and 10x Tesla's, on a stock that started the period under $9.
- GM returned **+17.1%**, a steady but modest gain.
- Tesla returned **+11.0%** — positive, but the least of the three despite far higher headline volatility.

### 📅 Monthly / Cumulative Trend
- Ford's rally builds steadily through 2021 and peaks around **+143.8% in December 2021**, driven by strong EV-transition news flow (Mustang Mach-E, F-150 Lightning) before giving some back into early 2022.
- Tesla actually spends much of **Q1–Q2 2021 in negative territory** (as low as −14.3% in May) before a strong recovery from October 2021 onward.
- GM's return path is the smoothest of the three — fewer sharp swings, a gradual climb, and a pullback into early 2022.

### 📉 Volatility & Risk
- **Tesla is the riskiest of the three**, with daily volatility of **3.64%** vs. 2.80% (Ford) and 2.47% (GM).
- Tesla's average daily trading range is **$36.36** — dramatically larger than Ford's $0.54 or GM's $1.69 (expected, given Tesla's much higher share price, but it still means bigger day-to-day dollar swings for holders).
- Tesla also owns both extremes: the **best single day** of the three (+19.6%, Mar 9 2021) and the **worst** (−12.0%, Nov 9 2021).

### 🔗 Correlation
- Ford and GM move together closely (**correlation 0.76**) — both are legacy automakers reacting to the same sector and macro news.
- Tesla is only weakly correlated with either (**0.22 with Ford, 0.25 with GM**) — it behaves more like a separate, tech-driven asset than a "third automaker."
- **Practical takeaway:** pairing Tesla with a legacy automaker gives more real diversification than holding two legacy automakers together.

### 📦 Trading Volume
- Ford had by far the **highest total trading volume** (24.5B shares) — consistent with its low share price and high retail trading interest.
- Tesla (8.0B) and GM (5.7B) traded far less by share count, though Tesla's dollar volume is much larger given its price.

## 🛠️ Tools & Technologies

- Python (pandas, numpy)
- DAX (Power BI-style measures — see `DAX_Measures.txt`)
- Excel (`DAX_Ford_Stock.xlsx`, `DAX_GM_Stock.xlsx`, `DAX_Tesla_Stock.xlsx`, `DAX_Stocks_Combined.xlsx`)
- Chart.js (interactive HTML dashboard)
- Data Cleaning & Transformation
- Financial Analysis (return, volatility, correlation)
- Data Storytelling

## 📈 Dashboard Features

The interactive dashboard includes:

- KPI Cards (trading days, total volume, best performer, avg. volatility)
- Cumulative Return by Month (3-line comparison chart)
- Total Return % Comparison
- Total Volume Traded (by company)
- Volatility / Risk Comparison
- Average Daily Trading Range
- Best & Worst Single-Day Movers table
- Return Correlation table

## 💡 Recommendations

Based on the analysis:

1. **Ford led on total return** in this window — its EV pivot narrative drove sustained upside that neither GM nor Tesla matched over the same period.
2. **Tesla carries the most risk** — anyone holding it should expect the largest single-day swings of the three, in both directions.
3. **Ford and GM aren't a diversified pair** — their 0.76 correlation means they tend to rise and fall together; combining Tesla with either offers more balance.
4. **GM was the "steady" stock** — lower volatility, smoother trend, more modest return — a reasonable lower-risk pick of the three.
5. Further work: extend the window past Feb 2022 to see whether Ford's outperformance held up through the 2022 market downturn.


##  Files in This Repo

| File | Description |
|---|---|
| Interactive dashboard |
| `README.md` | This file |
| `DAX_Ford_Stock.xlsx` / `DAX_GM_Stock.xlsx` / `DAX_Tesla_Stock.xlsx` | Per-company cleaned data with calculated columns (Daily Return %, Cumulative Return %, Moving Averages) |
| `DAX_Stocks_Combined.xlsx` | All three companies in one workbook, one sheet each |
| `DAX_Measures.txt` | Power BI DAX measure definitions behind every dashboard metric |
| `Ford_GM_Tesla_Stock_Dashboard.pptx` | Slide presentation summarizing the analysis |
# Stock-Performance-Dashboard
Stock performance dashboard comparing Ford, GM, and Tesla using returns, volatility, and correlation analysis
