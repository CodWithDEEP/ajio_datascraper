Ajio Scraper:
   The Ajio Scraper is a Python script that allows you to scrape product data from the Ajio website. It retrieves information such as        product names, IDs, prices, and links for a specific category.

Prerequisites:
   Before running the script, ensure that you have the following dependencies installed:

    Python 3.x
    Requests library (pip install requests)
    Pandas library (pip install pandas)
    
 Usage:
    To use the Ajio Scraper:

    Instantiate the AjioScraper class:


scraper = AjioScraper()
Call the all() method to initiate the scraping process and save the data to a CSV file:

The scraped data will be saved in a CSV file named ajio__data.csv in the current directory.

Customization:
You can customize the scraping process by modifying the following attributes in the AjioScraper class:

base_url: The base URL of the Ajio API. You can change it to scrape data from different categories.
page_size: The number of products to retrieve per page. Adjust it based on your requirements.
Notes
The script will scrape data from 20 pages of the specified category. You can modify the range in the scrape_data() method to scrape more or fewer pages.
The script uses the Ajio API to retrieve the data in JSON format. It extracts the relevant information and stores it in a list.
The scraped data is then converted into a Pandas DataFrame and saved as a CSV file for further analysis or processing.
