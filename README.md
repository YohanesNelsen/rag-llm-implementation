# Data Engineering Individual Project
## Overview
This project provides a web scraper for extracting reviews and additional infromation from Steam and SteamDB using Microsoft Edge browser. It utilizes a Jupyter Notebook along with EdgeDriver for automation. The scraper is designed to fetch reviews for a specified Steam game ID.

# Steam Web Scraping
## Requirements
Microsoft Edge browser <br>
Jupyter Notebook <br>
EdgeDriver <br>

## Setup
Download and install Microsoft Edge browser if you haven't already. <br>
Ensure Jupyter Notebook is installed in your environment. <br>
Download EdgeDriver and place it in the edgedriver folder. <br>

## Usage
Open the Jupyter Notebook in your preferred environment. <br>
Update the Steam game ID in the notebook to the desired game you want to fetch reviews for. <br>
- In this project, only 3 game are used to make it more simple yet scalable <br>

Run the notebook. The scraper will automate Microsoft Edge to extract reviews for the specified game. <br>
Note that the results may vary each time the notebook is run as the data on Steam is regularly updated. <br>

## Note
It is important to keep EdgeDriver up to date for compatibility with the Microsoft Edge browser. <br>
This web scraper does not extract Steam account ID to protect user data.

# Data Cleaning
## Requirement
All csv files from web scraping <br>
Jupyter Notebook <br>

## Usage
Run the notebook, and the result will be combined_reviews.csv, combined_pricing.csv, and combined_game_info.csv
