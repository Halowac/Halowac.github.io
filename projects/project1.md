[Back to Portfolio](./)

# Python Job Board Web Scraper

* **Class:** CSCI 301 - Survey of Scripting Languages
* **Grade:** A
* **Language(s):** Python
* **Source Code Repository:** [CSCI_301-Webscraper](https://github.com/Halowac/CSCI_301-Webscraper) *(Please email me to request access.)*

---

## Project Description

This project is a web scraping tool developed in Python that automates the extraction of recent job postings published on the official Python website (`https://www.python.org/jobs`). The script parses the HTML code of the page using the BeautifulSoup library to extract key information from each job listing, including the job title, hiring company, geographic location, posting date, category, and required job type. The collected data is processed and displayed in the terminal.

---

## How to Run the Program

Since this programming language does not require compilation, you can run the program directly from the terminal by following these steps:

1. Ensure you have Python installed and the following dependencies installed (`requests` and `beautifulsoup4`):
   ```bash
   pip install requests beautifulsoup4
   ```
2. Navigate to the directory where the script is located and execute it with the following command:
   ```bash
   python CSCI_301-Webscraper.py
   ```

---

## UI Design

Since this is a command-line interface application, user interaction takes place entirely through the terminal. The program processes the webpage and outputs a numbered list containing the details of each available vacancy.

Upon launching, the script sends an HTTP `GET` request to the Python Jobs URL and begins parsing the structured content of the job listings.

![screenshot](images/launch.png)
* **Fig 1.** The properties of each job offer are printed to the console in readable text format.

![screenshot](images/exception.png)
* **Fig 2.** If a network connection issue occurs or the server is unavailable, the script throws an exception from the `requests` library indicating the request failure.

---

## 3. Additional Considerations

The script handles potential variations in the HTML structure of the target webpage, such as extra lines in the company name using string cleaning methods like `splitlines()` and `.lstrip()`.

[Back to Portfolio](./)
