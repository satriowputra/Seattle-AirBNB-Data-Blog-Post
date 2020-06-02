### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)

## Installation <a name="installation"></a>

Please make sure that wordcloud library is installed on your system prior using the notebook. There are also several libraries that i used here that should be installed if you are install Python from Anaconda Distribution.

## Project Motivation<a name="motivation"></a>
In this project, I want to apply my knowledge as Data Scientist to explore and gain insight from Airbnb Seattle data. I cleaned and analyzed the data I got from this [Kaggle Dataset](https://www.kaggle.com/airbnb/seattle/data). I am using Matplotlib to visualize findings and Wordcloud to show what is matter inside each neighbourhood. To fill missing values, i am using several methods which are:
1. Forward fill and Backward fill to treat missing values in "price" column. I sorted the data based on listing_id and date before filling the data using mentioned method.
2. Mean and mode filling to fill missing values in some column such as "bathrooms", "cleaning_fee", and other columns. Please find it on notebook I provided here.

Last, I used Random Forest Regressor to find features that are useful to predict rent price. I also used AdaBoost Regressor but I found that Random Forest algorithm has the better result.

## File Descriptions <a name="files"></a>

Dataset used is from Airbnb Seattle. You can download it [here](https://www.kaggle.com/airbnb/seattle/data) or find it on this repository. There are three files which are calendar.csv, listings.csv, and reviews.csv.

## Results<a name="results"></a>

I have provided the notebook here in the repository. Uncomment "savefig" if you want to save generated plot.

Result summary:
1. I find the vibe for each neighbourhood using Wordcloud.
2. Price is hiking in busiest time of the year which is summer 2016. The price was rising 16% or 20$ from the price on early 2016.
3. Overall visit trend to Seattle is declining.
4. Number of bedrooms, accommodates, and bathrooms are top features to predict how much do we need to pay for a night in out host. The more bedrooms, the higher the price.  

You can find detailed finding on my blog post on [Medium](https://medium.com/@satriowputra/airbnb-seattle-story-1a71e08a805f?source=friends_link&sk=7c9e021ce5d84483910d17273e07bd31).
