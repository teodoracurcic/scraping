# Homework 07: Web Scraping with BeautifulSoup
Lede Program 2025 — [ledeprogram.com](https://ledeprogram.com)

This assignment includes four scraping tasks using Jupyter Notebook.

## Summary by Notebook

### `homework-7-part1.ipynb`
- **Task**: Scrape the **list of U.S. presidents** from Wikipedia.
- **Libraries**: `pandas`
- **Approach**: Used `pandas.read_html` to directly read the table from the page (no need for `requests` or `BeautifulSoup`).

### `homework-7-part2.ipynb`
- **Task**: Scrape article data from **Le Monde** homepage.
- **Libraries**: `requests`, `BeautifulSoup`, `pandas`
- **Collected**: Title, subhead, article URL, byline, article type, image URL, and whether it’s premium.

### `homework-7-part3.ipynb`
- **Task**: Scrape **authorized third-party driver license locations** from the Arizona Department of Transportation website.
- **Libraries**: `requests`, `BeautifulSoup`, `pandas`
- **Details**: Extracted structured data from `<td>` elements including company name, address, phone, hours, and website URL (when available). User-Agent headers were required to access the page.

### `homework-7-part4.ipynb`
- **Task**: Scrape **search results** from the Tennessee Western Bankruptcy Court website.
- **Libraries**: `requests`, `BeautifulSoup`, `pandas`, `os`
- **Extracted**: Case name, case URL, category, and additional details (terms matched, file size, PDF URL).  
- **Bonus**: Downloaded all case PDF files using the scraped URLs.