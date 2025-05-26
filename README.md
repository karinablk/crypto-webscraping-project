# Memecoin Market Analysis – Web Scraping & Exploratory Data Project

This project focuses on collecting and analyzing data from the memecoin section of CoinMarketCap using Selenium, BeautifulSoup, and a public API. The objective was to explore the speculative nature of memecoins by comparing them with major cryptocurrencies such as Bitcoin, Ethereum, and Solana.

## Project Objective

The goal was to examine the behavior, volatility, and data quality of memecoins. Particular attention was paid to differences between verified and unverified tokens, and to identifying how these assets differ from established cryptocurrencies in terms of risk and reliability.

## Dataset Overview

This project is based on two custom-built datasets collected from [CoinMarketCap](https://coinmarketcap.com):

- **Memecoins dataset**  
  • 1,552 rows  
  • 15 variables (e.g. price, market cap, supply, popularity)  
  • Scraped using BeautifulSoup & Selenium  
  • Mainly reflects current values at the time of scraping

- **Top cryptocurrencies dataset**  
  • 3,621 rows  
  • 5 variables (e.g. date, price, market cap)  
  • Fetched via public API  
  • Timeframe: 1 year of historical daily data

> **Note:** Only the cleaned `memecoins_clean.csv` file is included in this repository (`/data/`). The rest of the data was processed directly during scraping/API calls and not saved separately.

## Key Challenges

- Dynamic HTML structure of CoinMarketCap (frequent changes in element IDs/classes)  
- Missing or inconsistent values (e.g. N/A market caps, unverified tokens)  
- Merging data from heterogeneous sources (live web + API)  
- Filtering and cleaning data before analysis

## Workflow Summary

- Web scraping using Selenium and BeautifulSoup  
- API data collection for BTC, ETH, SOL  
- Data cleaning and merging  
- Exploratory data analysis of volatility, correlation, and outliers  
- Comparison between memecoins and top cryptocurrencies  
- Visualization of key trends and observations

## Repository Structure

- `notebook_web_scraping.ipynb`: scraping, cleaning and analysis notebook  
- `data/`: cleaned dataset `memecoins_clean.csv`  
- `web_scraping_project_presentation.pdf`: summary slides  
- `requirements.txt`: list of required libraries

## Conclusions

The analysis confirmed that memecoins are highly volatile and often lack consistent financial data, especially compared to established cryptocurrencies. Verified tokens tend to show more stability, while many unverified coins exhibit erratic price and volume behavior.

Although scraping provided full control over data selection, using a structured API would be more reliable for production environments, given how dynamic and unstable the structure of CoinMarketCap’s website can be. However, this project was intended as a demonstration of web scraping techniques and handling real-world data imperfections.
