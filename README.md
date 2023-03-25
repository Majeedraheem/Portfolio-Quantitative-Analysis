![alt text](./challege_4/Images/portfolio-analysis.png)



# Background :

investing in algorithmic trading strategies is the way to determine how, why, and which portofilo to invist in. 
quantitative analysis techniques with Python and Pandas,  determine which portfolio is performing the best across multiple areas: volatility, returns, risk, and Sharpe ratios.

# Prepare the Data

First, you will read in and clean several CSV files for analysis. The CSV files contain data on whale portfolio returns, algorithmic trading portfolio returns, and S&P TSX 60 historical prices. Use the Whale Analysis starter code to complete the following steps:
Use Pandas to read the following CSV files into DataFrames. Be sure to convert the dates to a DateTimeIndex.
whale_returns.csv: Contains returns of some famous "whale" investors' portfolios.
algo_returns.csv: Contains returns from the in-house trading algorithms from your company.
sp_tsx_history.csv: Contains historical closing prices of the S&P TSX 60 Index.
Identify and remove null values.

Remove any non-numeric values (e.g., dollar signs) from the DataFrames and convert the data types as needed.
The whale portfolios and algorithmic portfolio CSV files contain daily returns, but the S&P TSX 60 CSV file contains closing prices. Convert the S&P TSX 60 closing prices to daily returns.
Join Whale Returns, Algorithmic Returns, and the S&P TSX 60 Returns into a single DataFrame with columns for each portfolio's returns.
returns-dataframe.png

# Perform Quantitative Analysis

Analyse the data to determine if any of the portfolios outperform the stock market (that is, the S&P TSX 60). Specifically, you will do a performance analysis and a risk analysis, and then calculate rolling statistics and Sharpe ratios.
Performance Analysis

Calculate and plot daily returns of all portfolios.
Calculate and plot cumulative returns for all portfolios. Does any portfolio outperform the S&P TSX 60?
Risk Analysis

Create a box plot for each of the returns.
Calculate the standard deviation for each portfolio.
Determine which portfolios are riskier than the S&P TSX 60.
Calculate the annualised standard deviation.
Rolling Statistics

Calculate and plot the rolling standard deviation for all portfolios, using a 21-day window.
Calculate and plot the correlation between each stock to determine which portfolios mimic the S&P TSX 60.
Choose one portfolio, then calculate and plot the 60-day rolling beta between that portfolio and the S&P TSX 60.
Rolling Statistics Challenge: Exponentially Weighted Average

An alternative method to calculate a rolling window is to find the exponentially weighted moving average. This is like a moving window average, but it assigns greater importance to more recent observations. Try calculating the ewm Links to an external site. with a 21-day half-life.
Sharpe Ratios

Investment managers and their institutional investors look at the return-to-risk ratio, not just the returns. After all, if you have two portfolios that each offer a 10% return, yet one is lower risk, you would invest in the lower-risk portfolio, right? Follow these steps:
Using the daily returns, calculate the Sharpe ratios and visualise them in a bar plot.
Determine whether the algorithmic strategies outperform both the market (S&P TSX 60) and the whales portfolios.
Create a Custom Portfolio

