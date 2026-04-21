# AAPL vs TSLA Monthly Return Comparison (2020-2022)

## 1. Problem & User
Help investors compare the monthly return volatility of Apple (AAPL) and Tesla (TSLA) between 2020 and 2022, to understand which stock is riskier and which offers more extreme returns.

## 2. Data Source
- **Source**: WRDS CRSP Monthly Database (`crsp.msf` + `crsp.msfhdr`)
- **Access Date**: April 14, 2026
- **Key Fields**: `date` (date), `ret` (monthly return), `htsymbol` (ticker)

## 3. Methods
- Connect to WRDS using `wrds` library and query data with parameterized SQL
- Data cleaning: filter missing returns, sort by date
- Analysis: descriptive statistics (mean, standard deviation), extreme return identification
- Visualization: Matplotlib line chart

## 4. Key Findings
- TSLA monthly return volatility (std ≈ 24.92%) is much higher than AAPL (≈ 9.69%)
- Both dropped sharply in March 2020 (COVID-19), TSLA fell more (-21.56% vs -6.98%)
- TSLA had extreme positive return (+55.52%) in January 2021

## 5. How to Run
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open `assignment-2.ipynb`, fill in your WRDS credentials (or use provided CSV files)
4. Run all cells (or view pre-saved outputs)

## 6. Product Link / Demo
- GitHub Repository: https://github.com/JunnanPang/acc102-stock-analysis
- Demo Video: [Link to your YouTube video]

## 7. Limitations & Next Steps
- Only two stocks and three years of data, not generalizable
- No control for market benchmark (e.g., S&P 500)
- Next: expand to more stocks, add benchmark, build Streamlit app
