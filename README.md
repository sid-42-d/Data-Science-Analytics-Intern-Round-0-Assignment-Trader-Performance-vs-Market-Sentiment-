# Trader Performance vs Market Sentiment Analysis

Analyzing the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader behavior on Hyperliquid exchange. Examines 184,263 trades from 32 accounts to identify profitable patterns and predict high-performance trading days.

## Key Results
- **XGBoost Model**: 76.58% accuracy predicting high-profitability days
- **Best Strategy**: Contrarian shorting during greed periods (+$87/trade avg)
- **Worst Condition**: Neutral sentiment (31% win rate, highest overtrading)

## Repository Structure
```
├── Trader_Performance_vs_Market_Sentiment.ipynb    # Main analysis notebook
├── Output chart and tables/                        # All visualizations & results
│   ├── *.png                                       # Performance charts
│   └── *.csv                                       # Data tables
├── data/                                           # Project documentation
├── README.md                                       # Project documentation
└── LICENSE                                         # MIT License
```

## Requirements
- Python 3.8+
- pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost

## Setup & Installation

### 1. Clone Repository
```bash
git clone https://github.com/sid-42-d/Data-Science-Analytics-Intern-Round-0-Assignment-Trader-Performance-vs-Market-Sentiment-.git
cd Data-Science-Analytics-Intern-Round-0-Assignment-Trader-Performance-vs-Market-Sentiment-
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

### 3. Download Data Files

Download the required datasets:

**Bitcoin Market Sentiment (Fear/Greed Index):**
```
https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing
```

**Hyperliquid Trading Data:**
```
https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing
```

Place downloaded files in your working directory or update file paths in the notebook accordingly.

## How to Run

### Google Colab (Recommended)
1. Upload `Trader_Performance_vs_Market_Sentiment.ipynb` to [Google Colab](https://colab.research.google.com/)
2. Mount Google Drive and update file paths in the notebook
3. Run all cells: `Runtime > Run all`


## Analysis Workflow
1. **Data Preparation** - Load, clean, merge sentiment & trading data
2. **Performance Analysis** - Compare outcomes across Fear/Greed conditions  
3. **Behavioral Analysis** - Examine position sizing, aggression, directional bias
4. **Trader Segmentation** - Classify into Frequent/Infrequent, High/Low Volume
5. **Predictive Modeling** - XGBoost classifier (76.58% accuracy)

## Key Findings
- **Performance Paradox**: Win rate ≠ profitability (position sizing matters more)
- **Contrarian Success**: Shorting greedy markets yields highest profits
- **Neutral Danger**: Worst performance during unclear sentiment (overtrading)

## Outputs
All visualizations and data tables available in `/Output chart and tables/`:
- Performance metrics by sentiment
- Behavioral analysis charts
- Trader segment comparisons
- Model feature importance
- Summary statistics (CSV format)

## Actionable Strategies
1. **Short during Greed** - Increase short positions 20-30% when Fear/Greed Index hits 60-75
2. **Avoid Neutral Days** - Reduce trading 50% when index is 45-55 (highest overtrading risk)

## License
MIT License - see LICENSE file

## Contact
[Siddhant Pastapure] - [pastapuresiddhant24@gmail.com]
