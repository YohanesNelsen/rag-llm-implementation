# Data Engineering Individual Project
## Overview
This project utilise data from Steam, a popular online market for pc games. I webscrape several information, clean it, utilise apache spark and apply RAG and LLM to analise it.

# Requirements
Microsoft Edge browser <br>
Compatible version of EdgeDriver for webscrapping <br>
Ai8 Platfom for LLM and RAG implementation <br>
All folders from this project must be downloaded

# Steam Web Scraping
This part provides a web scraper for extracting reviews and additional infromation from Steam and SteamDB using Microsoft Edge browser. It utilizes a Jupyter Notebook along with EdgeDriver for automation. The scraper is designed to fetch reviews for a specified Steam game ID.

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
This section outlines a process for cleaning the data obtained through "Web Scraping" and merging it into three final databases, which are prepared for further processing.

## Usage
Run the notebook, and the result will be combined_reviews.csv, combined_pricing.csv, and combined_game_info.csv

# RAG & LLM
This section implements RAG (Red, Amber, Green) analysis and LLM (Log-Linear Modeling) using the data that has already been processed.

## Usage
Ensure you have the data cleaning folder with the cleaned datasets and the API key for the preffered LLM <br>
For this notebook, it is optimised to used in Ai8 <br>
Run the notebook associated with this section. Ensure all necessary dependencies are installed <br>
Follow the instructions within the notebook to execute the RAG and LLM analysis on the processed data
