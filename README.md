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

**_2._** In a second step the numcerical and categorcials are further processed
* Notebook: *numericals_categoricals.ipynb* At the end this step saves a cleaned csv file.
* for instance amenities is a list of strings, this code creates a boolean if an amenity is available in the accomodation or not

**_3._** Data is visualized in different graphs with the main aim to show which hosts or listings use airbnb professionally instead of its intended use
* Notebook: *data_visualization_2.ipynb*
* comments describe most of the findings within the notebook

**_4._** Uses Kmeans clustering to find patterns in the data 
* the aim was to create cluster that distinguish between professional listings and ocasionally rented out accomodations
* Notebook: *easy_kemans_cluster_test1.ipynb* uses only continious numerical data for kmeans. 
* Notebook: *kmean_clustering_2.ipynb* uses also boolean data, which is not an optimal solution for the Kmeans algortihm, however gives a better result in this case
* especially cluster 1 has profesional listings: entire homes, hosts other listings, many reviews per month (high activity)
* especially cluster 2 has more less profesional listings: private rooms, shared bathroom

* columns that have outliers like the price are for instance log transfromed


![alt text](https://github.com/MarcelMB/Covid19_school_closure_monioring_analysis/blob/main/example_figure_1.png)





## Data source:

http://insideairbnb.com/get-the-data.html

Using the detailed csv file of Berlin airbnb listings
