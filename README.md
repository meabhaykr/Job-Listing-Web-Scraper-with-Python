# Job-Listing-Web-Scraper-with-Python

This Python script is designed to scrape job listings from the JobInventory website based on a search query and location. It uses the `requests` library to send GET requests to the website, `BeautifulSoup` for parsing HTML, and regular expressions to clean up the extracted data. The job details are then stored in a CSV file for future use.

## Prerequisites

Before running the script, make sure you have the following prerequisites installed:

- Python: This script is written in Python, so you need to have Python installed on your system.

- Python Libraries: Install the required Python libraries using the following:

  ```bash
  pip install requests beautifulsoup4 pandas
  ```

## Usage

1. Define your search query and location by modifying the `search_query` and `location` variables at the beginning of the script.

2. Adjust the `max_pages` variable to determine how many pages of job listings you want to scrape. In the example provided, it's set to 5, but you can change it to any desired number.

3. Run the script by executing it in your Python environment.

4. The script will send GET requests to JobInventory, scrape job listings, and clean up job descriptions.

5. A CSV file named "job_listings_multiple.csv" will be created in your working directory, containing the scraped job details.

6. You can access the scraped job listings in the Pandas DataFrame `df`, and the CSV file can be used for further analysis.

## Customization

Feel free to customize the script according to your specific requirements. You can change the base URL, add more fields to scrape, adjust the regular expressions for data cleaning, or modify the output format as needed.

## Important Notes

- Web scraping may be subject to website terms and conditions, so use this script responsibly and make sure to respect the website's rules.

- Websites may change their structure over time, which can affect the script's functionality. Ensure that the HTML structure on JobInventory.com hasn't changed if you encounter issues.

- You can schedule this script to run at regular intervals to keep your job listings data up to date.
