# Flipkart Scraper
In this project, I have made a flipkart scraper in which I have scraped a minimum of 10 pages of the products Redmi and Oppo Android Mobiles using Selenium, BautifulSoup and requests. As scraping from all 10 pages will take some time, and to make it faster I used the concurrency method with the modules concurrent and multiprocessing. I have scraped Name, Price, RAM Info, Ratings, Product URL and it's description and stored it in JSON file at the end.

## Requirements

### BeautifulSoup

Beautiful Soup is a Python package for parsing HTML and XML documents. It creates a parse tree for parsed pages that can be used to extract data from HTML, which is useful for web scraping. If you're using Linux based OS, you can install BeautifulSoup using following command in terminal.

Here, pip is a package-management system used to install and manage software packages written in Python.

```
sudo apt-get update && sudo apt-get install python3-pip
pip3 install beautifulsoup4
```
### Selenium

The selenium package is used to automate web browser interaction with Python. I used selenium to open the flipkart site, search android mobiles and then apply filter by brand name and then passed the page source to BeautifulSoup.

You can install Selenium module by following command in teminal in Linux.

```
pip3 install selenium
```
To establish the connection between Chrome and Selenium, we need to use ChromeDriver.

You can install chromedriver by following command:

```
pip3 install chromedriver
```



### Requests Library

Requests is an Apache2 Licensed HTTP library, written in Python. Requests will allow you to send HTTP/1.1 requests using Python.
You can install requests library using following code in your terminal in Linux.

`pip3 install requests`

After finishing installation process above, you can run the tasks, using `python3 flipkart_scrap.py` and you will get your data stored in flip_scrap.json.
