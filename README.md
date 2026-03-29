# Analyzing Historical Stock & Revenue Data — Dashboard Project

A three-part data science project that demonstrates how to extract, process, and visualize historical stock and revenue data using Python. The project covers two extraction techniques — API-based retrieval and web scraping — culminating in an interactive financial dashboard.

---

## Project Structure

| Notebook | Description |
|----------|-------------|
| `Lab_1-Extracting_Stock_Data_Using_a_Python_Library.ipynb` | Extract stock data using the `yfinance` library |
| `Lab_2-Extracting_Stock_Data_Using_a_Web_Scraping.ipynb` | Extract stock data via web scraping with `BeautifulSoup` |
| `Lab_3-Extracting_and_Visualizing_Stock_Data.ipynb` | Full pipeline: extract + visualize Tesla & GameStop data |

---

## Lab Summaries

### Lab 1 — Python Library (yfinance)
- Connect to Yahoo Finance using the `yfinance` `Ticker` API
- Retrieve stock metadata (country, sector, market cap)
- Extract full historical share price and dividend data
- Visualize price trends using `matplotlib`
- **Stocks:** Apple (AAPL), AMD (AMD)

### Lab 2 — Web Scraping (BeautifulSoup)
- Send HTTP requests and parse raw HTML with `BeautifulSoup`
- Navigate HTML table tags (`<tbody>`, `<tr>`, `<td>`) to extract structured data
- Load results into Pandas DataFrames
- Compare manual scraping vs. `pd.read_html()` shortcut
- **Stocks:** Netflix (NFLX), Amazon (AMZN)

### Lab 3 — Extraction & Visualization (Capstone)
- Combine `yfinance` and web scraping in a single workflow
- Extract quarterly revenue data by scraping HTML pages
- Clean and transform raw data (strip currency symbols, handle nulls)
- Build interactive dual-panel dashboards using `Plotly`
- **Stocks:** Tesla (TSLA), GameStop (GME)

---

## Technologies Used

- **Python 3.8+**
- `yfinance` — Stock data via Yahoo Finance API
- `requests` + `BeautifulSoup` — Web scraping
- `pandas` — Data manipulation
- `plotly` — Interactive visualization
- `matplotlib` — Static plotting

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/JomolJudit/stock-data-analysis.git
cd stock-data-analysis

# Install dependencies
pip install yfinance requests bs4 html5lib lxml pandas plotly matplotlib

# Launch Jupyter
jupyter notebook
```

Then open each lab notebook in order.

---

## Key Concepts Demonstrated

- Fetching financial data from REST APIs
- HTML parsing and structured data extraction
- Data cleaning (currency formatting, null handling)
- Time-series visualization
- Building interactive dashboards with Plotly subplots
