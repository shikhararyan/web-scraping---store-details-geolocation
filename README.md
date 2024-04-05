# Retail Store Location Scraper - V-Mart

This project involves scraping the location details of V-Mart retail stores including address, area, contact number, coordinates, timing, and directions from the official V-Mart website. It utilizes web scraping techniques with Python libraries such as requests, BeautifulSoup, and pandas.

## Libraries Used:
- **requests**: For making HTTP requests to the website and retrieving the HTML content.
- **pandas**: For data manipulation and analysis.
- **re**: Built-in library for working with regular expressions.
- **BeautifulSoup**: For parsing HTML documents and extracting relevant information.

## Steps:
1. **Sending GET Request**: A GET request is sent to the V-Mart website to fetch the HTML content of the store locations page.
2. **Parsing HTML**: BeautifulSoup is used to parse the HTML content and navigate through the structure of the webpage.
3. **Extracting Information**:
    - **Address and Area**: Extracted from specific HTML elements.
    - **Contact Number**: Extracted from anchor tags with `tel:` href attribute.
    - **Timing**: Extracted from span tags with specific class names.
    - **Location Links**: Extracted from anchor tags with child i tags of a particular class.
    - **Coordinates**: Extracted from location links using regular expressions.
4. **Creating DataFrame**: All extracted information is stored in a pandas DataFrame.
5. **Storing Data**: The DataFrame is exported to a CSV file named `data.csv`.
6. **Downloading CSV**: The CSV file is downloaded for further analysis.

## Usage:
To run the scraper and fetch the latest store location details, simply execute the provided Python script.

## Note:
Ensure compliance with website terms of service and legal requirements while scraping data.
