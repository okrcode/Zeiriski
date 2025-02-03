# Zeiriski
This script is designed to scrape data from the Japanese website "zeirishikensaku.jp." It involves interacting with the website using both requests and Selenium for handling cookies and submitting forms. The primary objective is to retrieve data about agriculture and income in various prefectures.

# Key Steps:
## Initial Setup: The script defines headers and functions to initiate cookies and URLs for different prefectures.
## Data Fetching: Using requests, it posts form data to retrieve page information, iterating over different prefectures and checkbox values.
## Selenium for Cookie Management: When the requests approach faces issues, Selenium is used to simulate user interaction and fetch necessary cookies.
## Multithreading: Data fetching is done concurrently using ThreadPoolExecutor for improved performance when scraping multiple prefectures and checkboxes.
## Data Parsing: The data is parsed using lxml and stored for further processing.
