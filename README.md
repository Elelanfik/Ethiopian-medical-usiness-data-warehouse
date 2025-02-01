# Ethiopian-medical-usiness-data-warehouse

## Overview
This project involves building a data warehouse to store and analyze data on Ethiopian medical businesses scraped from Telegram channels. The goal is to create a robust and scalable data architecture utilizing modern data engineering practices including ETL/ELT processes, and object detection using YOLO.

## Table of Contents
- [Project Setup](#project-setup)
- [Tasks](#tasks)
  - [Task 1: Data Scraping and Collection Pipeline](#task-1-data-scraping-and-collection-pipeline)
  - [Task 2: Data Cleaning and Transformation](#task-2-data-cleaning-and-transformation)
  - [Task 3: Object Detection Using YOLO](#task-3-object-detection-using-yolo)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Project Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/Elelanfik/Ethiopian-medical-business-data-warehouse.git
    cd Ethiopian-medical-business-data-warehouse
    ```

2. Set up a virtual environment and install necessary dependencies:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

## Tasks

### Task 1: Data Scraping and Collection Pipeline
- **Objective**: Set up a pipeline to scrape data from Telegram channels using Beautiful Soup, Scrapy, and Selenium.
- **Steps**:
  1. Use Telegram API or write custom scripts to extract data.
  2. Implement storage of raw data in a temporary location.
  3. Monitor and log the scraping process.
- **Relevant Channels**:
  - [DoctorsET](https://t.me/DoctorsET)
  - [Chemed Telegram Channel](https://t.me/lobelia4cosmetics)
  - etc.

### Task 2: Data Cleaning and Transformation
- **Objective**: Clean and transform the scraped data for better usability.
- **Steps**:
  1. Remove duplicates and handle missing values.
  2. Standardize data formats.
  3. Store cleaned data in a database.
  4. Use DBT for data transformation.
    ```bash
    dbt run
    ```

### Task 3: Object Detection Using YOLO
- **Objective**: Implement object detection to extract useful insights from images.
- **Steps**:
  1. Set up the YOLO environment and install required libraries.
  2. Download YOLO model and prepare image data.
  3. Use the YOLO model to detect objects in the collected images and process detection results.

## Technologies Used
- Python
- Beautiful Soup
- Scrapy
- Selenium
- YOLO (You Only Look Once)
- DBT (Data Build Tool)
- PostgreSQL


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


