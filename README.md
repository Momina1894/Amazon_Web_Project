For this project, I utilized BeautifulSoup to web scrape data from a book listing on Amazon, specifically the book titled "How I Became Stupid" by Martin Page. The goal was to automate the extraction of key information from the webpage, including product details, pricing, and customer reviews, among other relevant data points. The raw HTML content of the page was first downloaded using the requests library, which allowed for a seamless interaction with the webpage.

Once the HTML was obtained, BeautifulSoup (BS4) was used to parse the data and extract the specific elements needed. This involved navigating through the HTML structure of the page to identify and isolate the desired information, such as:

Product Title: The title of the book, which is essential for identifying the product.
Pricing Information: The current price of the book, which can fluctuate and is vital for tracking over time.

To achieve the automation, a script can be scheduled to run at regular intervals, such as daily, using tools like cron jobs (on Unix-based systems) or Task Scheduler (on Windows). This script will:

Access the Amazon webpage: Download the latest HTML content using the requests library.
Parse the HTML: Extract the relevant data using BeautifulSoup.
Store the Data: Append the extracted data to a CSV file, creating a historical log of the information.


This approach provides a powerful method to track how the book’s market presence evolves over time. It can be particularly useful for monitoring pricing trends, understanding customer sentiment through reviews, and keeping a record of any changes in product availability or description. Additionally, this project can be expanded or adapted to scrape similar data from other products or websites, providing a scalable solution for automated data collection.

Here’s the link to the specific page being scraped: [How I Became Stupid on Amazon.](url)
