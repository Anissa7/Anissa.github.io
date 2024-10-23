# Web Scraping Assignment - Group 8

### Group 8
- Anissa
- Isaiah
- Johnson
- Elvis

### Links:
- [Google doc](https://docs.google.com/document/d/1RPMdGYzplcRXmdZ530BnKXBqGLgbSflz-7derB74qVk/edit?usp=sharing)

- [Video Presentation](https://www.loom.com/share/a68d395b4d814916aa1da48eec812577?sid=e34c40a3-12f3-4f3c-8d7b-cf09dc383ddc)


## Introduction

This repository contains the implementation of various web scraping tasks using Python libraries such as `BeautifulSoup`, `requests`, and `PIL`. The project involves scraping data from websites, processing HTML content, and saving relevant data to CSV files or images to categorized folders.

## Tasks Overview

### Task 0: Star Wars Ships API Integration (Isaiah)

- **Objective**: Fetch and list ships capable of carrying a given number of passengers from the Star Wars API (SWAPI).
  
- **Function**: `availableShips(passengerCount)` takes an integer `passengerCount` as input and returns a list of ships that can carry the specified number of passengers.

- **Sample Output**:  
  `['Death Star', 'Executor', 'Droid control ship', 'AA-9 Coruscant freighter', 'Republic Assault ship', 'Trade Federation cruiser']`

---

### Task 1: Web Scraping from a Sports Site (Anissa & Elvis)

- **Objective**: Scrape data from [Scrape This Site](https://www.scrapethissite.com/pages/forms/) and extract tabular information about hockey teams, including wins, losses, and goals.

- **Steps**:
  1. Make a request to fetch the webpage using the `requests` library.
  2. Parse the HTML content using `BeautifulSoup`.
  3. Locate the table and extract the rows and columns.
  4. Store the extracted data in a pandas DataFrame.

- **Sample Data**:
  | Team Name          | Year | Wins | Losses | Win % | Goals For (GF) | Goals Against (GA) | + / - |
  |--------------------|------|------|--------|-------|----------------|--------------------|-------|
  | Boston Bruins       | 1990 | 44   | 24     | 0.55  | 299            | 264                | 35    |
  | Buffalo Sabres      | 1990 | 31   | 30     | 0.388 | 292            | 278                | 14    |
  | Calgary Flames      | 1990 | 46   | 26     | 0.575 | 344            | 263                | 81    |
  
- **Output**: The extracted data is saved to a CSV file `data.csv`.

---

### Task 2: Amazon Product Images Scraping (Johnson & Isaiah)

- **Objective**: Scrape product images from different categories (Electronics, Baby, Shoes, Watches, Cameras) on Amazon, and store them in corresponding folders.

- **Steps**:
  1. Create a request to Amazon categories.
  2. Fetch and save the first 5 product images from each category using `requests` and `PIL`.
  3. Handle potential errors such as status code failures (e.g., 503 errors for certain categories).

- **Categories Scraped**: 
  - **Baby**: Successfully scraped and saved images, including Pampers, HelloBaby, and The Honest Company.
  - **Other Categories**: Failed due to access issues (HTTP 503 errors).

- **Sample Output**:
  - Category: **Baby**
    - Product: Pampers  
      Image URL: `https://m.media-amazon.com/images/I/61Kcg05Sz4L._AC_UL320_.jpg`
    - Product: HelloBaby  
      Image URL: `https://m.media-amazon.com/images/I/61WoQMri81L._AC_UL320_.jpg`

---
