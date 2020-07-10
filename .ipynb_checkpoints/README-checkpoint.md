# Capstone: Check In 4

### Contents:
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data Sources](#Data-Sources)
- [Data Dictionary](#Data-Dictionary)
- [Conclusions/Recommendations](#Conclusions)

<a id=Problem-Statement></a>
## Problem Statement: 
Do certain types of venues in an area correlate with the average real estate prices in that area.

<a id=Executive-Summary></a>
## Executive Summary: 
#### Goal  
The goal of this project is to determine if there is a correlation betweent ypes of venues in an area and the average real estate prices in that area.  The area of focus is Santa Clara County in California.
#### Data  
Location data was obtained by webscraping Wikipedia for a list of cities in the California Bay Area. (https://en.wikipedia.org/wiki/List_of_cities_and_towns_in_the_San_Francisco_Bay_Area)
Real Estate data detailing the average prices per city in Santa Clara County. The data provided was in a pdf which could not be scraped.  Data was copied directly into a csv file for upload.(https://www.sccaor.com/pdf/stats/2019.pdf)
Venues for each city were obtained from Foursquare using an API. (https://api.foursquare.com/v2/venues/explore)
#### Metrics     
Principal Component Analysis (PCA) was used to model the data.  Success metrics include the R2 Score and Mean Squared Error (MSE)
#### Findings
There is not a strong correlation between venues types and average housing prices.

#### Risks/Limitations/Assumptions
This subset of venue types and housing prices may be too small and too uniform to determine if there is a correlation.






