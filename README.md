# Bitcoin Market Sentiment vs. Trader Performance Analysis

## 📌 Project Overview
This project explores the relationship between Bitcoin market sentiment (as measured by the Crypto Fear & Greed Index) and actual trader performance using historical trade data from the Hyperliquid platform. The goal is to identify whether market psychology is a reliable predictor of trader profitability, risk appetite, and participation.

## 📊 Datasets
- **Bitcoin Market Sentiment Dataset (`fear_greed_index.csv`)**: Daily sentiment classifications ranging from "Extreme Fear" to "Extreme Greed."
- **Historical Trader Data (`historical_data.csv`)**: High-frequency trade logs including execution price, size (USD), side, and Closed PnL.

## 🛠️ Methodology & Technical Steps
1. **Data Cleaning**: Resolved timestamp unit mismatches (converted milliseconds to proper datetime objects) and handled missing PnL values.
2. **Aggregation**: Aggregated millions of individual trades into daily metrics (Average PnL, Win Rate, Volatility) to align with daily sentiment readings.
3. **Merging**: Performed an inner join on calendar dates to create a unified analysis dataset.
4. **EDA**: Visualized distributions, boxplots for trade size, and correlation matrices to identify hidden patterns.

## 💡 Key Insights & Deductions
- **The Extreme Greed Edge**: Counter-intuitively, "Extreme Greed" periods showed the highest win rate (~47%), significantly outperforming all other sentiment regimes (~33%).
- **The Participation Paradox**: Trader activity (unique accounts) peaked during "Extreme Fear" phases, suggesting that the traders in this dataset act as contrarians/bottom-fishers.
- **Volatility Trends**: Bullish periods (Greed/Extreme Greed) exhibited the lowest PnL volatility, while "Extreme Fear" was associated with massive, unpredictable swings.
- **Profitability Mismatch**: There was a near-zero correlation (0.04) between the raw sentiment score and average profitability, proving that sentiment influences *behavior* more than it guarantees *returns*.

## 🚀 How to Run
1. Ensure `pandas`, `seaborn`, and `matplotlib` are installed.
2. Place the datasets in the root directory.
3. Run the `[Your_Filename].ipynb` notebook sequentially.

## ⚠️ Limitations
- The "Extreme Fear" insights are based on a relatively small sample size (~14 days) and should be treated as preliminary.
- The dataset is heavily influenced by high-volatility events in early 2025.
