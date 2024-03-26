# Building an Equal-Weight S&P 500 Index Fund
Welcome to the Equal-Weight S&amp;P 500 Index Fund project! In this project, we aim to create a Python script that will help you construct an equal-weight version of the S&amp;P 500 index fund. By doing so, you can achieve diversification across all constituents of the index without having to manually calculate the weights for each stock.
## Introduction
The S&P 500 index is widely regarded as one of the most important benchmarks for the performance of the U.S. stock market. It consists of 500 of the largest publicly traded companies in the United States, spanning various industries and sectors. The SPDR® S&P 500® ETF Trust, with over US$250 billion in assets under management, is one of the largest funds that track this index.

The traditional method of weighting in the S&P 500 index fund is market capitalization-weighted, meaning that companies with higher market capitalizations have a larger influence on the index's performance. However, in this project, we will focus on creating an equal-weight version of the index fund.
## Library Imports
To accomplish this project, we will utilize various Python libraries for data manipulation, analysis, and visualization. Here are the primary libraries we will be using:

* pandas: For data manipulation and analysis.
* requests: For making HTTP requests to retrieve stock data.
* beautifulsoup4: For web scraping to obtain the constituent stocks of the S&P 500 index.
* numpy: For numerical computing.
* matplotlib: For data visualization.

![image](https://github.com/ansalm98/Equal-Weight-S-P-500-Index-Fund-Project/assets/47536642/808c3531-d24b-4075-8e20-9d4f7d87eef1)
These libraries will enable us to retrieve stock data, perform calculations, and visualize the results effectively as we construct the equal-weight S&P 500 index fund.
Importing S&P 500 Constituents and Making API Calls
In this section, we'll begin by importing the constituents of the S&P 500 index. We have a static version of the S&P 500 constituents available, and we'll use this data to proceed with our analysis. Additionally, we'll import our IEX Cloud API token, which is the data provider we'll be using throughout this project.

## Importing S&P 500 Constituents
The S&P 500 constituents change over time, and in an ideal scenario, we would connect directly to the index provider (Standard & Poor's) to pull their real-time constituents regularly. However, for this project, we have a static version of the constituents available.

## Download the Constituents: S&P 500 Constituents
Move the File: Move the downloaded file into the starter-files folder so it can be accessed by other files in that directory.

## Acquiring an API Token
We'll be using the IEX Cloud API to retrieve market capitalization and stock prices for each S&P 500 constituent. It's essential to store API tokens and other sensitive information securely.

## Making Our First API Call
We need to structure our API calls to IEX Cloud to retrieve the required information, including market capitalization and stock prices for each stock.

## Parsing Our API Call
The data retrieved from the API call isn't in the proper format yet. We need to parse it first before proceeding.

## Adding Stocks Data to a Pandas DataFrame
We'll create a Pandas DataFrame to store the stock's price and market capitalization data. Think of a DataFrame like the Python version of a spreadsheet, allowing us to store tabular data efficiently.

## Looping Through the Tickers
Using a loop, we'll pull data for all S&P 500 stocks and store their data in the DataFrame.

## Using Batch API Calls to Improve Performance
Batch API calls can significantly improve the performance of our code, as HTTP requests are typically slow. We'll split our list of stocks into groups of 100 and make batch API calls for each group.

## Calculating the Number of Shares to Buy
Next, we'll calculate the number of shares of each stock to buy to achieve an equal-weight version of the S&P 500 index fund.

## Formatting Our Excel Output
We'll utilize the XlsxWriter library to create nicely-formatted Excel files. This library offers extensive customization options, allowing us to create professional-looking outputs.

## Creating the Formats for Our .xlsx File
We'll define formats for tickers, stock prices, market capitalization, and the number of shares to purchase.

## Applying the Formats to the Columns
We'll apply the defined formats to specific columns of our Excel spreadsheet.

## Saving Our Excel Output
Finally, we'll save our formatted Excel output, which will contain the recommended trades for an equal-weight S&P 500 index fund.
