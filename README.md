# Airbnb_Berlin_analysis

This analysis was performed as part of a project week within the Ironhack Data Analysis Bootcamp.

It includes analysis of web-scraped data from airbnb.com and a KMeans clustering approach.

## Motivation
Airbnb is a wonderful possibility to travel and discover the local life by living in a place that a local person rents out.

However, some people also use airbnb as their primary income, increasing rental prices in the neigborhood and contribruting to the shrotage of liavable space within cites.

Airbnb does not share the data. However, it is possible to analyze data that is publicly available on their webpage.

## How to use?

The analysis code is based on several jupyter notebooks.  

**_1._** In a first step the dataset is cleaned and summarized 
* Notebook: *data_cleaning_selection.ipynb* At the end this step saves a cleaned csv file.
* Mostly dealing with NaNs
* clean string columns which incldue numericals
* droping unnessecary data columns

**_2._** In a first step the dataset is cleaned and summarized 

**_3._** Uses Kmeans clustering to find patterns in the data 
* the aim was to create cluster that distinguish between professional listings and ocasionally rented out accomodations
* Notebook: *data_cleaning_selection.ipynb* At the end this step saves a cleaned csv file.

## Data source:

http://insideairbnb.com/

Using the detailed csv file of Berlin airbnb listings
