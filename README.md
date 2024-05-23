# Web Scraper for Quotes

This project is a simple web scraper built with Python that extracts quotes and their authors from the website Quotes to Scrape and saves them into a CSV file.

## Prerequisites

Before running the script, ensure you have the following installed:

- Python 3.x
- pip (Python package installer)
- Virtual environment (recommended)

## Installation

1. Clone the Repository:

   ```
   git clone https://github.com/nigelseah24/python-web-scraper.git
   cd python-web-scraper/
   ```

2. Create and Activate a Virtual Environment:

- Windows:

  ```
  python -m venv venv
  .\venv\Scripts\activate
  ```

- macOS and Linux:
  ```
  python3 -m venv venv
  source venv/bin/activate
  ```

3. Install Required Packages:

   ```
   pip install -r requirements.txt
   ```

   Create a requirements.txt file with the following content:

   ```
   requests
   beautifulsoup4
   ```

## Usage

1. Run the Script:

   ```
   python scraper.py
   ```

   This will fetch quotes and authors from Quotes to Scrape and save them into quotes.csv.

2. Output:

   The quotes and their authors will be printed in the terminal and also saved in a CSV file named quotes.csv.

## Script Details

The scraper.py script performs the following steps:

1. Sends an HTTP GET request to fetch the HTML content of the quotes page.
2. Parses the HTML content using BeautifulSoup.
3. Extracts quotes and authors using CSS selectors.
4. Writes the extracted quotes and authors to a CSV file named quotes.csv.

## Example Output

Example output in the terminal:

```
"The greatest glory in living lies not in never falling, but in rising every time we fall." - Nelson Mandela
"The way to get started is to quit talking and begin doing." - Walt Disney
...
```

Example content of quotes.csv:

```
Quote,Author
"The greatest glory in living lies not in never falling, but in rising every time we fall.",Nelson Mandela
"The way to get started is to quit talking and begin doing.",Walt Disney
...
```

## Acknowledgements

The quotes and authors are fetched from Quotes to Scrape.
