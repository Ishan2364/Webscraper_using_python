# Web Scraper for Extracting News Articles

This script fetches and extracts article content from the Economic Times website using Python's `requests` and `BeautifulSoup` libraries.

## Features
- Retrieves the web page content.
- Parses and extracts the main article content.
- Cleans the extracted text for readability.
- Displays the article content in the console.

## Requirements
Ensure you have the required dependencies installed:

```bash
pip install requests beautifulsoup4
```

## Usage
Run the script in Jupyter Notebook:

```python
!python scraper.py
```

## How It Works
1. The script sends a GET request to the provided article URL.
2. If the request is successful (status code 200), it parses the HTML content using BeautifulSoup.
3. It selects the article text using a CSS selector (`div.article-content > p`).
4. The extracted text is cleaned and displayed.

## Example Output
```
NVIDIA stock is down by 27% from its peak...
Here's what to expect next.
```

## Notes
- The article structure may change, requiring updates to the CSS selector.
- Ensure the target website allows web scraping (check `robots.txt`).

## License
This project is licensed under the MIT License.

