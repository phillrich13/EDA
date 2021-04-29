# MTA Rush Hour Traffic Exploratory Analysis

## Abstract
In this exploratory data analysis (EDA) project, the goal was to use [MTA data](http://web.mta.info/developers/turnstile.html) to understand rush hour traffic, with the end goal of better staffing stations. The process consisted of ranking stations on their average traffic (entries and exits), as well as the change in their traffic on a weekly basis. With these ranks, I was able to rank and group the highest and lowest traffic stations into deciles. This allows for creating high priority groups for staffing as well as low priority groups that should receive the minimum staffing. Future steps include setting up geographical boundaries for headcount allocation.

## Design
This project focused around the potential for increased rush hour ridership as NYC begins reducing Covid restrictions. With the reduction of restricitions comes the potential for increased station traffic, especially during typical rush hours. With the potential increase in station traffic comes the need for increased MTA staffing. By identifying high and low traffic stations, defined by total foot traffic and change in foot traffic week over week, more informed staffing decisions can be made. This also accounts for certain geographical areas getting back up to normal traffic standards quicker than high traffic stations with stagnant growth.

## Data
There were 2 data sets used in the project. The first and primary data set was the [MTA turnstile data](http://web.mta.info/developers/turnstile.html). The second data set was for [MTA Station Locations (long/lat)](http://web.mta.info/developers/developer-data-terms.html#data). The MTA data contained 14 weeks of entry asnd exit data by unique turnstile for a 4 hour window. This 4 hour window was used to isolate rush hour periods for a given station. The entries and exits values are cumulative (lifetime, or since last reset of count), requiring manipulation to retrieve the actual number of entries/exits in a given window. The station location data provides station name with longitude and latitude for a given station, as well as other data not relevant to the analysis at hand. This was used to plot the stations in tableau.

## Methods (algorithms)

