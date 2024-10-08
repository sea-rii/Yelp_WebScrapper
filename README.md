# Scrape 'n' Taste Chicago

- The Srape 'n' Taste Chicago is a Python script designed to collect restaurant data from Yelp for the Chicago area. 
- It uses the requests library to download web pages and BeautifulSoup to parse the HTML content. 
- The script collects information such as restaurant names, URLs, ratings, review counts, neighborhoods, tags, price ranges, and services, and saves this data into a CSV file.
  


## Features
- Scrapes restaurant data from Yelp
- Extracts details such as name, image, URL, rating, review count, neighborhood, tags, price range, and services
- Handles pagination to collect data from multiple pages
- Saves the scraped data into a CSV file
  


## Requirements
- Python 3.x
- requests library
- beautifulsoup4 library
  


## Installation
- Clone the repository or download the script.
- Install the required Python libraries:
  
     `pip install requests beautifulsoup4`


 ## Usage
- Open the script in a text editor or an IDE.
- Modify the 'pages_to_scrape' list to include the initial Yelp search URL if you want to start from a different page.
- Run the script:
  
     `python yelp_scraper.py`
- The script will scrape restaurant data from Yelp and save it into a file named 'restaurants.csv' in the same directory.



## Code Explanation
- Initialization: Sets up the list of pages to scrape and an empty list for visited pages and scraped items.
- Scraping Loop: Loops through the pages to scrape and processes each one.
- Extracting Data: Selects and extracts restaurant data from the HTML content.
- Handling Pagination: Discovers new pagination links and adds them to the queue.
- Saving Data: Writes the scraped data to a CSV file.


