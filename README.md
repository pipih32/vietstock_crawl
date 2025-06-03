# vietstock_crawl
Crawl and analyze stock market articles from Vietstock.vn for potential competitor program promotions using Selenium and Google Sheets.

# Vietstock Competitor Program Analyzer

This project automates the crawling of stock market news from [Vietstock.vn](https://vietstock.vn), identifies articles that may promote competitor programs, and logs structured information to a Google Sheet for internal analysis.

## Overview

- Crawl articles from https://vietstock.vn/chung-khoan.htm using Selenium
- Navigate pagination and extract article titles, links, and publication dates
- Optionally filter articles based on time (e.g., last 24 hours)
- Designed to integrate with LLM-based analysis (e.g., Gemini Flash API)
- Store structured output in Google Sheets via Google Service Account

## Technologies

- Python 3.10
- Selenium (automated crawling)
- Google Colab (runtime)
- Google Sheets API (gspread)
- Pandas, Requests

## Repository Structure

vietstock-competitor-analyzer/
├── vietstock_crawler.py       
├── requirements.txt            
├── README.md                    
└── assets/

## How to Run

1. Clone the repository or open the script in Google Colab
2. Set up your Google Service Account and share the Google Sheet with its email
3. Install dependencies: pip install -r requirements.txt
4. Run the script to:
- Crawl news articles from Vietstock
- Extract and store structured information to Google Sheets or Excel

## Output Format

Each article entry includes:
- Title
- URL
- Publication time
- Source site (Vietstock)
- Crawling timestamp

The output is saved in a tabular format in Google Sheets or `.xlsx` for local review.

## Notes

- Ensure the site layout of Vietstock.vn remains unchanged; otherwise, CSS selectors may need to be updated
- Make sure your Service Account key is securely stored and not shared publicly

## Contact

Developed by Hoàng Thị Mai Phương
Email: hmphuonggg32@gmail.com
