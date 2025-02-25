
# Amazon Product Scraper for Samsung Products

This Jupyter Notebook scrapes product information from Amazon's search results for "Samsung" and extracts details such as product titles, prices, and ratings. The data is then cleaned and saved to a CSV file for further analysis.

## Features
- **Web Scraping**: Extracts product details from Amazon search results.
- **Data Cleaning**: Filters out invalid entries (e.g., "Page 1 of 1" prices).
- **CSV Export**: Saves the cleaned dataset to `amaon_data.csv` (note the typo in the filename).

## Requirements
- Python 3.x
- Libraries: `beautifulsoup4`, `requests`, `pandas`, `numpy`

## Installation
1. Install the required libraries:
   ```bash
   pip install beautifulsoup4 requests pandas numpy


## Usage
1. Run the Jupyter Notebook `Main.ipynb`.
2. The script will:
   - Send a request to Amazon's search page for "Samsung".
   - Extract product links from the search results.
   - Scrape title, price, and rating from each product page.
   - Clean the data by removing entries with invalid prices.
   - Save the results to `amaon_data.csv`.

## Data Output
The final dataset includes the following columns:
- `title`: Product name.
- `price`: Product price (formatted as a string, e.g., `$499.99`).
- `rating`: Product rating (out of 5, extracted as a string like `4.5`).

Example output:
| title                                                | price     | rating |
|------------------------------------------------------|-----------|--------|
| SAMSUNG Galaxy S24 FE AI Phone, 128GB Unlocked...    | $499.99   | 4.5    |
| SAMSUNG Galaxy Buds 3 Pro AI True Wireless Blu...    | $249.99   | 4.1    |

## Notes
- **Selectors**: The script uses specific HTML class/ID selectors (e.g., `productTitle`, `a-offscreen`). These may change over time, requiring updates to the code.
- **User-Agent**: A valid `USER_AGENT` header is included to mimic a real browser request.


<div align="center">
<h1>🧑‍💻 Happy coding!</h1>
</div>


