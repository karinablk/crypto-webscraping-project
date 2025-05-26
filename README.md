# Memecoin Market Analysis – Web Scraping & Exploratory Data Project

This project focuses on collecting and analyzing data from the memecoin section of CoinMarketCap using Selenium, BeautifulSoup, and a public API. The objective was to explore the speculative nature of memecoins by comparing them with major cryptocurrencies such as Bitcoin, Ethereum, and Solana.

## Project Objective

The goal was to examine the behavior, volatility, and data quality of memecoins. Particular attention was paid to differences between verified and unverified tokens, and to identifying how these assets differ from established cryptocurrencies in terms of risk and reliability.

## Dataset Overview

**Source:** data was collected through live scraping of CoinMarketCap (memecoin category) and via a public API endpoint for BTC, ETH, and SOL historical data.  
**Structure:** merged dataset with coin name, price, market cap, 24h % change, and verification status.  
**Size:** small cleaned dataset available in `data/memecoins_clean.csv`

## Key Challenges

- Dynamic HTML structure on CoinMarketCap (inconsistent element IDs and tags)
- Missing or incomplete data (e.g. N/A values, missing volume or market cap)
- Combining scraped data with API results from different structures and formats

## Workflow Summary

- Web scraping using Selenium and BeautifulSoup
- API data retrieval and merging
- Data cleaning and formatting
- Exploratory analysis of volatility, correlation, and structure
- Comparison of memecoins vs. top cryptocurrencies
- Visualization and interpretation of results

## Repository Structure

- `notebook_web_scraping.ipynb`: scraping, cleaning, and analysis notebook  
- `data/`: cleaned CSV file with scraped data  
- `web_scraping_project_presentation.pdf`: presentation summary of the project  
- `requirements.txt`: list of libraries used
