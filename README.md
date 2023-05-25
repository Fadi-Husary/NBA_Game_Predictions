# NBA_Game_Predictions
This project is aimed at building a machine learning model to predict the outcome of an NBA team's next game based on historical game data. The project incorporates data collection via web scraping, data cleaning and preprocessing, feature engineering, and finally, the creation of a machine learning model for making predictions. An accuracy score of 63.58% was achieved using new features. 

The website used to scrape NBA data is [basketball-reference](https://www.basketball-reference.com/).

## File Descriptions:
1) NBA_stats_webscrape.ipynb: This file is code on web scraping from the above website to get NBA data html pages for years 2016-2023, and grab the box scores needed from each page.
2) NBA_stats_parse.ipynb: This file will have code on parsing through the box scores on every game between 2016 and 2023, and grabbing all of the needed data and turn them into a DataFrame and save them as a CSV file. 
3) NBA_game_preds.ipynb: This file will show how to take the data collected from the last two files and cleaning it up a little, adding new features, and training and testing the model. 


## Steps: 
1) Web Scraping and Data Parsing:Find classes and anchor tags to scrape data from [basketball-reference](https://www.basketball-reference.com/). Create 3 directoreis to store the html pages and box scores.
2) Data Cleaning and Preprocessing: Turn lists of data into a DataFrame, delete unnecessary columns, reset the index, add any needed columns, handle null values, etc.
3) Feature Engineering: Create new features that could potentially improve the accuracy of the model.
4) Model Training and Testing: A Ridge Classifier model is trained on the preprocessed data, and the model's performance is tested. A backtesting method is applied, where the model trains on past seasons and makes predictions for the current season. Finally, the accuracy of the model's predictions is computed.

## Installations and Packages:
- JupyterLab
- Python 3.8+
- Python packages:
     - pandas
     - scikit-learn
     - beautifulsoup4
     - playwright
