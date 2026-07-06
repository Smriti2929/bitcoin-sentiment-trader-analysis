# Bitcoin Sentiment vs Trader Performance Analysis

## Objective
Analyzing the relationship between Bitcoin Fear & Greed sentiment and 
trader performance using Hyperliquid historical trading data.

## Datasets
- `fear_greed_index.csv`: Daily sentiment classification (2018–2025)
- `historical_data.csv`: Trade-level execution data from Hyperliquid

## Key Findings
- Extreme Greed periods showed the highest win rate (~47%) compared to 
  ~33% across all other sentiment categories.
- Average PnL showed no strong linear correlation with sentiment score.
- Unique trader participation was highest during Extreme Fear, suggesting 
  contrarian trading behavior in this dataset.

## Limitations
- Extreme Fear category is based on a small sample (~14 days) and should 
  be interpreted with caution.

