Website-Scraper


This repository contains a simple and modular Python tool for scraping data from websites. Built as a command-line utility, it's designed to be easily adaptable for various web scraping tasks, from extracting text content to collecting links or other specific information.

Key Features
URL-based Scraping: Accepts a URL as a command-line argument.

Modular Design: The core scraping logic is encapsulated in a separate scraper.py file, making it easy to customize and reuse.

Data Extraction: Capable of extracting text, links, or other HTML elements from a webpage.

Minimal Dependencies: Uses popular and lightweight libraries for web scraping.

Technologies Used
Python 3

requests: For making HTTP requests to fetch the webpage content.

beautifulsoup4: For parsing the HTML content and navigating the document tree.

Installation
Clone the repository to your local machine:

Bash

git clone https://github.com/MaxMoya/Website-Scraper.git
cd Website-Scraper
Install the required dependencies using pip:

Bash

pip install -r requirements.txt
Usage
To use the scraper, run the main.py script from your terminal and provide the URL of the website you want to scrape as an argument.

Bash

python main.py <URL_TO_SCRAPE>
Example:
To scrape data from https://en.wikipedia.org/wiki/Web_scraping, you would run:

Bash

python main.py https://en.wikipedia.org/wiki/Web_scraping
The script will print the scraped data directly to the console.

How to Modify
The true power of this tool lies in its modularity. You can easily customize it to scrape different types of information.

Open the scraper.py file.

Locate the main scraping logic (e.g., where BeautifulSoup is used to find elements).

Change the find() or find_all() methods to target the specific HTML tags, classes, or IDs you are interested in.

Example Modification:
To scrape all <h1> tags instead of p tags, you would simply change the relevant line of code inside scraper.py from soup.find_all('p') to soup.find_all('h1').

File Structure
main.py: The entry point for the command-line tool. It handles the URL argument and calls the scraper.

scraper.py: Contains the core WebsiteScraper class with the logic for fetching and parsing the webpage.

requirements.txt: Lists all the Python library dependencies.
