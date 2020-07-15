# Capstone Project: Austin Neighborhoods, A Look at Venues and Real Estate Prices

### Contents:
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Metrics](#Metrics)
- [Data Sources](#Data-Sources)
- [Data Dictionary](#Data-Dictionary)
- [Limitations](#Limitations)
- [Conclusions](#Conclusions)

<a id=Problem-Statement></a>
## Problem Statement: 

Can nearby venues be used to predict whether the average price per square foot for a neighborhood in Austin, Texas is, on average, less or greater than 400 dollars per square foot.

<a id=Executive-Summary></a>
## Executive Summary: 
 
The goal of this project is to explor whether or not venue types in neighborhoods throughout Austin, Texas contribute to the average price per square footage of a home for that neighborhood. People who are interested in this information are those looking for what neighborhood to purchase a home in based on the right mix of price and nearby attractions for them.

Location data for 37 neighborhoods in Austin was obtained along with the average price per square foot and a compilation of venue types within a 1000 meter radius of the neighborhood's center. I ended up with a total of 263 unique venue types.  Names of neighborhoods was obtained from Wikipedia via web scraping, real estate data was obtained from neighborhoods.com via web scraping, and venue data was obtained from Foursquare using an API.

I treated this as a classification problem and grouped the prices into two (2) categories, one for real estate less than and average of 400 dollars per square foot and real estate that is, on average, greater than 400 dollars per square foot.

Two uncommon libraries were used in this project. Geopy was used to pull latitude and longitude coordinates for each city and Folium was used to visualize the locations of cities in a map.

<a id=Data-Sources></a>
#### Data Sources

Location data was obtained by webscraping Wikipedia for a list of neighborhoods in Austin, Texas. (https://en.wikipedia.org/wiki/List_of_Austin_neighborhoods)
Real Estate data detailing the average prices per square foot per neighborhood was obtained from  neighborhoods.com (https://www.neighborhoods.com)
Venues for each neighborhood were obtained from Foursquare using an API. (https://api.foursquare.com/v2/venues/explore)

<a id=Data Dictionary></a>
## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**Neighborhood**|*object*|df_comb|Name of neighborhood|
|**Venue Type**|*object*|df_comb|Name of each venue type|
|**Price Group**|*int*|df_comb|0 for price <400/sq.ft. and 1 for >400/sq.ft.|

<a id=Metrics></a>
#### Metrics    

Several models were applied to the problem.  I used Principal Component Analysis (PCA), Support Vector Machines (SVM), Decision Trees, and Logistic Regression.  The Decision Tree model performed the best with a Testing Accuracy score of 0.875.  SVM and Logistic Regression both scored 0.625 on the Testing Accuracy.
Since the data set is so large with a total of 263 columns representing venue types I am using PCA to explain the results. The success metrics for PCA include an R2 Score of 0.23 and Mean Squared Error (MSE) of 0.18.

<a id=Limitations></a>
#### Limitations
There were several challenges in this project.  For one, getting a complete set of data was not possible.  Either geopy did not return coordinates or neighborhoods.com did not have sales data.  This resulted in going from and original list of 59 neighborhoods to 37.  Additionally, a dataset of neighborhoods in just one city yields a small test set.  This became less of an issue when I turned my target into a binary classification instead of 20 price ranges. 

<a id=Conclusions></a>
#### Conclusions
Using PCA to assess the impact of venues types on real estate prices, the venue types with the most positive correlation or effect are:
- Italian Restaurant
- Art Gallery
- Seafood Restaurant
- Ice Cream Shop
- Spa

Venue types with the most negative effect are:
- Pool Hall
- Camera Store
- Auto Dealership
- Bagel Shop
- Indian Restaurant

Venue types with the least correlation are:
- Playground
- Platform
- Tennis Court
- Kitchen Supply Store
- Golf Driving Range








