# Primetrade.ai: Bitcoin Sentiment & Trader Analysis

An end-to-end data science pipeline and interactive dashboard analyzing the relationship between Bitcoin market sentiment (Fear/Greed Index) and quantitative trader performance on the Hyperliquid exchange. 

Built as an analytical assessment to uncover hidden trading patterns, evaluate risk-taking behavior (leverage and position sizing) during emotional market extremes, and formulate data-driven Web3 trading strategies.

---

## 🛠 Tech Stack

* **Language:** Python 3
* **Environment Management:** `uv` (Lightning-fast package manager)
* **Data Processing:** `pandas`
* **Visualization:** `matplotlib`, `seaborn`, `plotly`
* **Interactive Dashboard:** `streamlit`
* **Exploratory Environment:** Jupyter Notebook

---

## 📂 Project Structure

This project was developed in 5 structured phases:

1.  **Data Ingestion:** Initialized the environment and loaded the sentiment and trade datasets.
2.  **Time-Series Alignment:** Standardized datetime formats and utilized `pd.merge_asof` to accurately map continuous trade executions to daily market sentiment states.
3.  **Exploratory Data Analysis (EDA):** Visualized distributions of leverage, position sizes, and closed PnL across different Fear/Greed classifications.
4.  **Pattern Discovery:** Grouped historical data at the account level to identify "Smart Money" outperformance and formulate actionable, mean-reversion trading strategies.
5.  **Interactive Dashboard:** Deployed a Streamlit web application to dynamically filter and visualize the findings.

---

## 🚀 Setup & Installation

**1. Clone the repository**
```bash
git clone <your-github-repo-link>
cd primetrade-sentiment-analysis
```

**2. Environment & Dependencies:**
This project uses uv for fast dependency management (defined in pyproject.toml).

```bash
# If using uv:
uv sync

# Alternatively, if using standard pip:
pip install -r pyproject.toml 
```

**3. Data Placement:**
Ensure you have downloaded the required datasets and placed them in a data/ directory at the root of the project:

```bash
data/bitcoin_sentiment.csv

data/hyperliquid_trades.csv
```

**4. Usage:**
*Running the Exploratory Notebook*

To view the detailed step-by-step analysis, data merging, and static visualizations:

1. Open analysis.ipynb in your preferred Jupyter environment (VS Code, JupyterLab, etc.).

2. Run the cells sequentially to generate the cleaned merged_data.csv file.


**5. Key Findings & Strategy**

**Leverage vs. Emotion:** Analysis reveals distinct correlations between extreme market greed and average leverage utilized by retail accounts.

**Contrarian Profitability:** "Smart money" accounts consistently reduce risk exposure during extreme greed and scale into positions during panic events.

Further detailed insights are available within the jupyter notebook.


##  Author

**Mohammad Taqreem Khan**