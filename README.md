# Stock-Performance-Analysis
Stock Performance Analysis Report
Project Overview
This project uses the power of Python for data preparation and analysis, along with Power BI for interactive and dynamic visualization, to provide deep insights into stock performance. The dashboard tracks key financial metrics, such as Daily Returns, Volatility, and Moving Averages, and includes visualizations that help users understand stock trends, assess risks, and make informed investment decisions.

The dataset consists of the following columns:
- Date: The trading date
- Open: The opening price of the stock on a particular day
- High: The highest price of the stock on that day
- Low: The lowest price of the stock on that day
- Close: The closing price of the stock
- Adj Close: The adjusted closing price, which accounts for stock splits, dividends, and other adjustments
- Volume: The number of shares traded
- Company: The company name to differentiate between multiple stocks

Data Preparation and Analysis Using Python
Python played a critical role in the data preparation and analysis phases of the project. Below are the key steps performed using Python:
1. Data Preprocessing
•	Loading the dataset: The dataset, containing columns for Date, Open, High, Low, Close, Adjusted Close, and Volume, was loaded and cleaned in Python.
•	Handling Missing Data: Missing values were identified and handled appropriately, either through interpolation or filling with relevant statistics.
•	Feature Engineering: Additional features such as Daily Returns, Volatility, and Rolling Averages were created.
Python Libraries Used:
•	pandas for data manipulation.
•	numpy for numerical operations.

2. Calculation of Metrics
Moving Average 
To analyze stock trends, two moving averages were calculated:
- 50-Day Moving Average: This captures the short-term trend of a stock's price over 50 trading days.
- 200-Day Moving Average: This captures the long-term trend of the stock's price over 200 trading days.
These moving averages help smooth out daily price fluctuations and highlight the stock’s general direction over time.

- Volatility Analysis: Rolling volatility, calculated using a 30-day rolling standard deviation, was used to track changes in volatility over time.
- Regression analysis: using StatsModels helps to model the relationship between the variables.
- Correlation Analysis: Pairwise correlations between stock prices, volumes, and returns were explored to understand how these factors interact.

3. Interactivity 
To enhance the user experience, interactive widgets (using `ipywidgets` in Jupyter notebooks) has been incorporated to allow users to filter data by company. This enables dynamic exploration of stock performance, allowing the user to select specific time periods to view trends, regressions, or volatility for a particular company.

Power BI for Visualization
After performing data preparation and analysis in Python, the results were imported into Power BI for visualization. Below are the key dashboards and visuals created in Power BI:
1. Key Performance Indicator (KPI) Cards
•	Current Stock Price: Displays the most recent closing price.
•	Price Change (Percentage) : Indicates how much the stock price has changed over a selected time period.
•	Average Daily Price: Shows the average trading price of for each stock.
•	Volume Traded: Visualizes the total volume of stocks traded over time.
2. Line Charts
•	Stock Price Trends: Line charts were used to visualize price trends over time, including overlaying the 30, 50, and 200-day moving averages to highlight long-term trends.
•	Volatility Trends: An area chart visualized how volatility changes over time, identifying periods of increased or decreased risk.
3. Rolling Volatility
•	Rolling volatility was plotted alongside stock prices to give a visual representation of the stock’s risk during different time periods.
Conclusion
This project integrates Python for advanced stock price analysis with Power BI for rich, interactive visualizations. By combining both tools, the dashboard provides investors and analysts with actionable insights into stock performance, volatility, and future price trends.
The integration of Daily Returns, Volatility, Moving Averages, and Regression Analysis allows for a comprehensive and highly visual stock analysis tool that can be adapted to any stock or dataset.

7. Future Work
There are several possible extensions to this analysis:
- Additional Indicators: The inclusion of technical indicators like the Relative Strength Index (RSI) or Moving Average Convergence Divergence (MACD) could provide more insight into stock momentum and potential price reversals.
- Sector-Wise Analysis: Grouping companies by sectors (e.g., technology, healthcare) could offer a more comprehensive analysis of how different industries perform relative to one another.
-Real-Time Data Integration: By integrating real-time stock data, this analysis could be adapted to provide live updates on stock performance, making it more applicable for day traders or active investors.

This project offers a robust framework for stock performance analysis and can be further extended to suit more complex use cases or larger datasets.

