# Final Project: Tesla & GameStop Stock and Revenue Dashboard

This repository contains scripts and notebooks to:

1. **Fetch historical stock data** using `yfinance`.
2. **Scrape quarterly revenue data** from Macrotrends via web scraping.
3. **Clean and process** the extracted data.
4. **Generate interactive dashboards** using Plotly.

---

## Repository Structure

```
├── tesla_revenue.py       # Scrapes Tesla revenue and displays last 5 rows
├── gamestop_revenue.py    # Scrapes GameStop revenue and displays last 5 rows
├── tesla_dashboard.py     # Fetches TSLA data, revenue, and plots dashboard
├── gamestop_dashboard.py  # Fetches GME data, revenue, and plots dashboard
└── README.md              # Project overview and usage instructions
```

---

## Prerequisites

- Python 3.7+
- Packages:
  - `yfinance`
  - `requests`
  - `pandas`
  - `beautifulsoup4`
  - `plotly`

Install dependencies via:

```bash
pip install yfinance requests pandas beautifulsoup4 plotly
```

---

## Usage

### 1. Tesla Revenue Extraction

```bash
python tesla_revenue.py
```
Prints the **last five quarters** of Tesla's revenue.

### 2. GameStop Revenue Extraction

```bash
python gamestop_revenue.py
```
Prints the **last five quarters** of GameStop's revenue.

### 3. Tesla Dashboard

```bash
python tesla_dashboard.py
```
Opens an interactive Plotly chart showing:
- Tesla stock closing price over time
- Tesla quarterly revenue on a secondary Y-axis

### 4. GameStop Dashboard

```bash
python gamestop_dashboard.py
```
Opens an interactive Plotly chart showing:
- GameStop stock closing price over time
- GameStop quarterly revenue on a secondary Y-axis

---

## Task Breakdown and Grading

| Task                                                         | Points |
|--------------------------------------------------------------|--------|
| 1. Tesla Stock Data Extraction (yfinance)                    | 2      |
| 2. Tesla Revenue Data Extraction (Web Scraping)              | 1      |
| 3. GameStop Stock Data Extraction (yfinance)                 | 2      |
| 4. GameStop Revenue Data Extraction (Web Scraping)           | 1      |
| 5. Tesla Stock & Revenue Dashboard                           | 2      |
| 6. GameStop Stock & Revenue Dashboard                        | 2      |
| 7. Notebook/Script Submission                                | 2      |
| **Total**                                                    | **12** |

---

## Notes

- Web scraping uses a simple `requests` + `BeautifulSoup` approach.
- Tables are identified by the presence of the "Revenue" header in the second column.
- Plotly dashboards use dual Y-axes for price vs. revenue comparison.

Feel free to explore and modify the scripts for other tickers or extended analyses!
