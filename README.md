# Crypto API Data Extraction

A Python-based automation script that pulls real-time cryptocurrency data from the CoinMarketCap API, normalizes the JSON output, and appends results to a timestamped CSV file for continuous tracking and analytics.

## Features
- Fetches live listings for top 5000 cryptocurrencies every 5 minutes
- Cleans and normalizes nested JSON data into a structured pandas DataFrame
- Appends each batch with a UTC timestamp to a CSV log for historical analysis
- Simple retry/exception handling for network stability

## Tech Stack
- Python (pandas, requests, json)
- CoinMarketCap API
- CSV-based local persistence

## Setup
```bash
# 1. Clone repo and install dependencies
pip install pandas requests

# 2. Run the data collector
python main.py
