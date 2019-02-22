# Twitter Data Analysis
This project was completed as part of the course requirements for Data Analyst Nanodegree with Udacity.

# Introduction

In this project we have wrangled and analysed data from a twitter account called WeRateDogs. This is a popular Twitter account with over 4 million followers and international media coverage that rates people's dogs with a humorous comment about the dog.  They have a unique system of rating, in which the denominator is almost always equal to 10, and the numerator almost always, greater than 10. 


# Project Description

Wrangled and analyzed data from the WeRateDogs Twitter account with 5000+ tweets. The data wrangling steps are documented in the **wrangle_report** pdf file.

Data wrangling consisted of the following stages:

## 1.	Gathering data:

The data was gathered from three different sources and in three different file formats.

i)	The first dataset was provided by Udacity and was downloaded manually. This was the WeRateDogs Twitter archive provided as a csv file: **twitter_archive_enhanced.csv**, and was loaded to a pandas dataframe.

ii)	The second dataset was the tweet image predictions file **image-predictions.tsv** that is hosted on Udacity's servers. The URL link was provided by Udacity and the file was downloaded programmatically using the Requests library, and read into a pandas dataframe.

iii)	Downloading and obtaining the third dataset was quite challenging. This required setting up a  up a Twitter developer account. We used the Tweepy library to query Twitter's API for additional data using the tweet ID of each tweet. The JSON data for all the tweets obtained using Python's Tweepy library was stored in a file called **tweet_json.txt file**, with each tweet's data in a single new line. Then this .txt file was read line by line into a pandas DataFrame.


## 2.	Assessing data:

After gathering data, the data was then assessed visually and programmatically. Several quality and tidiness issues were identified and documented for the three different input tables. As assessing and cleaning the entire dataset completely would be very time consuming, for the purpose of this project we identified approximately 8 quality issues 2 tidiness issues. These issues were then addressed and cleaned in the next stage. The quality and tidiness issues that were identified and addressed are documented in the **wrangle_report** pdf file.


## 3.	Cleaning data:

The various quality and tidiness issues identified were addressed and cleaned. Before the cleaning operations were performed, copies of the original datasets were made. The define, code, and test steps for each of the cleaning process were clearly documented. A tidy master dataset with all pieces of gathered data was created, and this was stored as a csv file **twitter_archive_master.csv** .

The tidy dataset **twitter_archive_master.csv** was subsequently analysed using python and its libraries to obtain interesting insights.


# Technologies Used

Python

Jupyter notebook

Python libraries - pandas, numpy, matplotlib, seaborn,os, json, tweepy,  requests


# Results

The results are documented in the **act_report** pdf file. 

To summarise, cleaned dataset was analysed and several interesting results and visualisations were obtained, including:

- Most common dog names

- Average dog rating, average favourite count and average retweet count

- Analysis of favourite_count and retweets according to dog stages

- Relation between Favourite Count and Retweet Count

- Some of the more popular dogs and the less popular ones along with their characteristics and dog type.
