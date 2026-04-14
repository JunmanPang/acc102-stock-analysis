# AAPL vs TSLA Monthly Return Comparison (2020-2022)

## 1. Problem & User
Help investors compare the monthly return volatility of Apple (AAPL) and Tesla (TSLA) between 2020 and 2022, to understand which stock is riskier and which has more extreme returns.

## 2. Data Source
- **Source**: WRDS CRSP Monthly Database (`crsp.msf` + `crsp.msfhdr`)
- **Access Date**: April 14, 2026
- **Key Fields**: `date` (date), `ret` (monthly return), `htsymbol` (ticker symbol)

## 3. Methods
- Connect to WRDS using the `wrds` library and query data with parameterized SQL
- Data cleaning: filter missing returns, sort by date
- Analysis: descriptive statistics (mean, standard deviation), extreme return identification
- Visualization: Matplotlib line chart to show return trends

## 4. Key Findings
- TSLA's monthly return volatility (std ≈ 18%) is much higher than AAPL's (≈ 8%)
- Both stocks dropped sharply in March 2020 (COVID-19 shock), with TSLA falling more (-21% vs -12%)
- TSLA had an extreme positive return (+45%) in January 2021, showing high elasticity

## 5. How to Run
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open `assignment.ipynb`, fill in your WRDS username and password in the connection cell
4. Run all cells sequentially (or simply view the pre-saved outputs)

## 6. Product Link / Demo
- GitHub Repository: https://github.com/JunnanPang/acc102-stock-analysis
- Demo Video: [Link to your YouTube video]

## 7. Limitations & Next Steps
- Only two stocks and three years of data, not generalizable
- Did not control for overall market effects (e.g., S&P 500 benchmark)
- Next steps: expand to more stocks, add industry comparisons, or build an interactive tool (Streamlit)
