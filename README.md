# Web Scraping and Analysis of Robots.txt Files

## Overview
This project collects and analyzes `robots.txt` files from a list of websites. The goal is to identify patterns in how different industries configure their crawlability rules. The script extracts `Allow` and `Disallow` rules and presents insights into website restrictions.

## Features
- **Web Scraping**: Fetch `robots.txt` from multiple websites using `requests`.
- **Parsing**: Extract `Allow` and `Disallow` rules from `robots.txt`.
- **Data Analysis**: Count and categorize restricted paths per website.
- **CSV Output**: Save results in a structured format for further analysis.

## Requirements
Install dependencies using:
```sh
pip install requests pandas
```

The output will include:
- **Console Display**: A summary table with allowed and disallowed path counts.
- **CSV File**: `robots_txt_analysis.csv` for further analysis.

## Example Output
| Website                | Allowed Paths | Disallowed Paths | Example Disallowed |
|------------------------|--------------|-----------------|--------------------|
| https://www.google.com | 89           | 248             | ['/search', '/sdch', '/groups'] |
| https://www.facebook.com | 84           | 686             | ['/', '/', '/'] |
| https://www.reddit.com | 0            | 1               | ['/'] |

## Insights
- **Social media platforms** have strict crawling restrictions.
- **E-commerce sites** block checkout and account-related pages.
- **News websites** restrict paywalled content but allow most articles.


