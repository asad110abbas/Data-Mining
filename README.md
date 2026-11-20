# 🗺️ BRIHA · Google Maps Data Mining

![Part of BRIHA](https://img.shields.io/badge/Part_of-BRIHA-8B5CF6?style=for-the-badge&labelColor=0B1024)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white) ![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-4B8BBE?style=flat-square) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

> ⚡ **Part of [BRIHA](https://github.com/asad110abbas)** · Briha Research, built by Syed Asad Abbas.

Automated **lead-generation scraper** that collects business listings from Google Maps search results
(name, rating, reviews, address, phone, website) and exports them as a clean dataset.

## Pipeline
```mermaid
flowchart LR
    A[Search query<br/>e.g. 'restaurants in Lahore'] --> B[Selenium + ChromeDriver<br/>auto-scroll results]
    B --> C[BeautifulSoup parsing]
    C --> D[Regex cleaning]
    D --> E[(pandas → CSV / Excel)]
```

## Highlights
- **Headless browser automation** with Selenium and `webdriver-manager` (no manual driver setup)
- **Infinite-scroll handling** to load every result, with polite delays
- **Robust parsing** with BeautifulSoup and regex for phone numbers, ratings and review counts
- **Analysis-ready output** as a pandas DataFrame exported to CSV / Excel

## Run
```bash
pip install selenium webdriver-manager beautifulsoup4 pandas requests
```
Open `Google_Map_Data_Mining.ipynb`, set your search query and run all cells. Chrome must be installed.

> Use responsibly and respect the website's terms of service and rate limits.
