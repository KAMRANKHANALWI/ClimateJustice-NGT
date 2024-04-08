```markdown
# Green Tribunal Case Records Scraper

## Table of Contents
- [Introduction](#introduction)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Files](#files)
- [Important Notes](#important-notes)
- [Support and Assistance](#support-and-assistance)

## Introduction
<p align="center"><img src="https://socialify.git.ci/KAMRANKHANALWI/ClimateJustice/image?font=Source%20Code%20Pro&amp;language=1&amp;name=1&amp;pattern=Circuit%20Board&amp;theme=Dark" alt="project-image"></p>

A short internship project at the interface of **#SemanticClimate** and **#IndiaJusticeReports** conducted at **#NIPGR**, New Delhi.

This Python script is designed to extract case details from [National Green Tribunal](https://www.greentribunal.gov.in/judgementOrder/zonalbenchwise) website using Selenium WebDriver and save them to a CSV file. The script navigates through the website, enters search parameters, solves CAPTCHA, extracts case details, and saves them to a CSV file.

## Dependencies
- **Selenium**: A Python library for automating web browsers.
- **Pytesseract**: Python binding to the Tesseract OCR engine for extracting text from images.
- **PIL (Python Imaging Library)**: Required for image manipulation.
- **Chrome WebDriver**: WebDriver for Chrome browser. Automatically managed by `webdriver_manager`.

## Usage
1. Ensure you have Python installed on your system and a code editor like VS Code to run the code.
2. Also, download ChromeDriver from [ChromeDriver Download Page](https://chromedriver.chromium.org/downloads)
3. Install the required dependencies using pip:
   ```
   pip install selenium pytesseract pillow webdriver-manager
   ```
4. Run the scripts using Python accordingly:
   ```
   python details.py
   ```
   ```
   python table.py
   ```

## How It Works
1. The script opens a Chrome browser and navigates to a specified URL.
2. It selects options from dropdown menus, captures a CAPTCHA image, extracts text from the image, and fills in the CAPTCHA field.
3. It enters search parameters such as date range and clicks the search button.
4. You can change the date range in the code accordingly like 'FROM DATE 03/03/2024 TO DATE 29/03/2024' by searching the word 'date' in VS Code (Ctrl + F)
5. It iterates through pagination and extracts case details for each page.
6. You can set the page range of which you want to extract the data like: 1 to 27 (goes till 26 pages
