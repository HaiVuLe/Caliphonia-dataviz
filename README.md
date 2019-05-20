# Caliphonia-dataviz

## Introduction

In this project, I analyzed the Vietnamese food landscape in California through data visualization using Tableau and Plotly.

Vietnamese food is what I'm proud of about my home country. Not only do I wish to introduce it to people around me, I am curious to explore how it is received, and hopefully loved, by people from all around the world. Additionally, understanding the food landscape in California, on another hand, would give me some insights into the life of the Vietnamese community here in the state with the biggest presence of Vietnamese population in the entire country. This is a topic that I personally care about.

A few questions I would like to explore include (1) where Vietnamese restaurants are, whether they are concentrated in areas with high representation of Vietnamese population or well spread across the state, (2) who are Vietnamese food consumers, how much is Vietnamese food loved by non-Vietnamese foodies, (3) what food is served and popular, and (4) what is the quality of Vietnamese restaurants here and how their cusomters received them.

![Map of Vietnamese restaurants in Californian cities](https://raw.githubusercontent.com/HaiVuLe/Caliphonia-dataviz/master/images/Chloropleth-what-counties.png)

## Data 

* Yelp data: The major source of data in this project is from Yelp. I used Yelp APIs and put together a dataset about Vietnamese restaurants in California. The data are search results returned by Yelp when querying "Vietnamese Restaurant in {city}, CA" with `city` being every city in California using the list of cities provided by [ESRI](https://www.esri.com/en-us/home). 

* US Census Bureau data: Besides, to enrich and contextualize my analysis, I used data of [population of Californian cities from the US Census Bureau (2018)](https://www.california-demographics.com/cities_by_population), and data of Vietnamese population by counties from the 2010 Demographic Profile Data dataset provided by the US Census Bureau. I also found a lot of useful information about the Vietnamese community here through the report ["The Vietnamese Population in the United States: 2010"](http://www.vasummit2011.org/docs/research/The%20Vietnamese%20Population%202010_July%202.2011.pdf) published at VA Summit (2011).

## What's in this repo

* [data](/data): includes data for all the plots generated. The csv files with naming convention `business_info_{city_name}` are raw data of restaurants from Yelp, each of which is for one city. For details of the data, see [Yelp documentation](https://www.yelp.com/developers/documentation/v3/business_search). A note is that the results for nearby cities may have overlap restaurants which should be removed for the correct count of restaurants.

* [images](/images): png files of the plots and maps.

* [data_scraping.ipynb](/data_scraping.ipynb): code to call Yelp APIs, parse json response into a pandas dataframe, and save it as csv files.

* [data-cleaning.ipynb](/data-cleaning.ipynb): remove duplicates and extract features.

* [Write up](/Vietnamese food landscape in California.pdf): write up of the analysis consisting of the data visualizations and the insight behind them.

* [final_project2.twb](final_project2.twb): Tableau notebook. 



