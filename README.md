# Banks-market-cap-analysis

This project is about using Python to gather data from the web about the largest banks in the world by market capitalization. I get the data from a Wikipedia page and clean it up so it’s easy to understand. The project uses web scraping to automate collecting this data, and then I organize it into a table for further analysis.

Steps in the Project,
01.ibrary Installation:
The first step involves installing necessary Python libraries:
Requests: To send HTTP requests and download the webpage content.
BeautifulSoup: To parse the HTML structure of the webpage and locate the desired table.
Pandas & Numpy: To clean, store, and process the data.

01.Web Scraping:
The project makes use of the Requests library to fetch the HTML content from a Wikipedia page. The URL is archived using the Wayback Machine to ensure data consistency (as web content can change over time).
Target URL: Archived Wikipedia page listing largest banks by market cap.

03.Data Extraction:
Using BeautifulSoup, the project locates the table of interest (containing bank names and market cap values) on the webpage.
The table rows are looped through, extracting the bank names and their respective market capitalization values.

03.Data Cleaning:
Market capitalization values are cleaned by removing symbols (like $, \n) and converted into float numbers.
The cleaned data is then added into a list and converted into a Pandas DataFrame.

04.Final DataFrame Output:
The final data is structured into a DataFrame with two columns:
Name: The name of the bank.
Market Cap (USD Billion): The market capitalization of the bank in billions of USD.


Technologies Used:
Python: To automate scraping and processing.
Requests & BeautifulSoup: For scraping the web data.
Pandas: To organize and clean the data.

Next Steps:
Visualization: The extracted data can be visualized.A
Automation: Extend this project to periodically scrape live data and automatically update the dataset, allowing for real-time tracking of changes in bank market capitalizations.
