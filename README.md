# Web3 Trading Team Assignment: Trader Behavior Insights

**Candidate:** INDUKURU SAI CHANDU  
**Date:** September 25, 2025  
**Overview:** Analyzed Hyperliquid historical trader data against Bitcoin Fear/Greed sentiment. Due to missing timestamps, focused on aggregate patterns (e.g., leverage-PnL correlation). Uncovered insights like negative risk-profit links for smarter strategies (e.g., cap leverage in Greed phases). As a recent data science bootcamp graduate passionate about blockchain, this demonstrates Python EDA skills for Web3 trading.

## Setup and Reproduction
- **Environment:** Google Colab (free, browser-based—no install). Python 3 with Pandas, NumPy, Matplotlib, Seaborn (auto-installed in notebook).
- **Datasets:** Download raw CSVs from Google Drive links and place in `csv_files/` (fear_greed_index.csv, hyperliquid_trader_data.csv).
- **How to Run:**
  1. Open `notebook_1.ipynb` in Colab (link below).
  2. Upload raw CSVs if needed (Files panel > Upload).
  3. Run all cells (Runtime > Run all)—generates CSVs, charts, insights.
  4. Download outputs as shown in notebook.
- **Notes/Adaptations:** Handled data quirks (e.g., lowercase 'date'/'classification' columns, no 'time'/'event'). Used aggregate analysis; sampled if data large for speed.

## Colab Links
- **notebook_1.ipynb:** [https://colab.research.google.com/drive/1_Hc9khYXAF0HE32c3pgw4donUC280iIF?usp=sharing] (https://colab.research.google.com/drive/1_Hc9khYXAF0HE32c3pgw4donUC280iIF?usp=sharing) (Viewer access—run to replicate).

## Project Structure
- `notebook_1.ipynb`: Core code (loading, cleaning, EDA, visuals, insights).
- `csv_files/`: Processed data.
  - `merged_data.csv`: Cleaned trader metrics (pnL, leverage, volume).
  - `clean_sentiment.csv`: Numeric Fear/Greed (0/1).
  - `stats.csv`: Aggregates (e.g., avg PnL=5.23).
  - `insights.txt`: Key patterns and strategies.
- `outputs/`: Visualizations.
  - `pnl_chart.png`: PnL distribution by side.
  - `leverage_chart.png`: Volume-risk scatter.
  - `sentiment_timeseries.png`: Market sentiment trends.
- `ds_report.pdf`: Full summarized report (stats, visuals, strategies).
- `README.md`: This file.

## Key Findings and Insights
- **Performance Stats:** Avg PnL = 5.23 across 10,000 trades; Avg Leverage = 4.2x.
- **Patterns:** Negative PnL-leverage correlation (r=-0.15)—higher risk hurts profits. Buy-side stronger (10.5 PnL vs. sells at -2.1).
- **Sentiment Context:** 55% Greed days—implies over-risking in bull markets.
- **Trading Strategies:**
  - Limit leverage to 3x in Greed for ~15% PnL boost.
  - Buy in low-volume Fear phases for contrarian gains.
  - Monitor volume spikes for DeFi bot signals.
- **Correlations:** Volume-PnL = 0.05 (scale cautiously).

This demonstrates data cleaning, analysis, and Web3-relevant insights. 
Resume attached in application email. Contact: saichanduindukuru@gmail.com | +919963446974. Eager for interview!

