---
title: "How Home Sale Prices Have Changed in NYC"
date: 2019-12-12
published: true
tags: [dataviz, altair, hvplot, holoviews, seaborn, websraping]
excerpt: "Visualising changes in home sale prices in New York City using data from Craigslist and the NYC Department of Finance. "
altair-loader:
  scraped_1_Scatter: "charts/plot1_craigslistPrices.json"
  scraped_2_MAP: "charts/plot2_craigslist_PricebyBorough.json"
  DOF_priceByBorough: "charts/plot3_prices_0915.json"
hv-loader:
  DOF_priceByZIPCODE: "charts/plot5_priceZipCode.html"
toc: true

toc_sticky: false

---

Home sale prices are a good indicator of gentrification as demand for housing in those areas increase and new developments are constructed. The amenities in these areas are also likely to improve, once again driving up sale prices. For the purpose of this analysis, data from the NYC Deparment of Finance Data (DOF) was used to analyze sale prices per zip code form 2009-2015. In order to get a proxy for current prices, Craigslist was scraped to home sale price data for 2019. 

## 2009-2015: Home Sale Prices by Zip Code

Past data was downloaded from the [Department of Finance]("https://data.cityofnewyork.us/City-Government/NYC-Citywide-Annualized-Calendar-Sales-Update/w2pb-icbu") and plotted using [Altair](https://altair-viz.github.io), [Seaborn](https://seaborn.pydata.org/index.html), and [Holoviews](https://hvplot.pyviz.org/). 

<u style="color: #f768a1"> Average Price per Square Foot across Boroughs and Years</u>
- The following plot was created using [Altair](https://altair-viz.github.io).
- Click on the legend to filter to specific categories of price/sqft! 
- Hover over each circle to get more information about the year, price/sqft and borough! 

<div id="DOF_priceByBorough"></div>

From the above plot, it is clear that houses in the Bronx and Staten Island have a lower price per square foot across all the years. Both prices in Brooklyn and Queens have bee increasing from 2009 to 2015, which could be indication of gentrification. Manhattan appears to have a very irregular trend in average price per square foot across the years. The next chart examines the relationship between the price and square feet for each of the Boroughs in each of the years 2009-2015. 

<u style="color: #f768a1">Hexbin Facetgrid comparing Price of Housing to Size for each Borough over Years</u>
- The following plot was created using [Seaborn](https://seaborn.pydata.org/index.html). 
- Each individual plot is the Sale Price vs Gross Square Feet of each listing from the data. 
- The entire facet grid shows the Boroughs (Rows) vs Years (Columns), and the same color scheme for the Boroughs is followed as from the previous chart. 

![Hexbin FacetGrid]({{site.url}}{{site.baseurl}}/assets/images/plot4_Size_to_price_ByBoroughYear.png)

The relationship between the sale price to size is much less steep for the Bronx and Staten Island. In Brooklyn, we notice that over the years, the concentration of price to size becomes progressively streamlined and steeper, indicating that there is an increase in overall sale price per square feet. This could be an indication of rising land value, one of the effects of gentrification. We also notice that Manhattan has a rather wide range housing prices to size, and this could be a reason for the rather fluctuating average price per square feet over the years in the previous chart. Nonetheless, many of the Manhattan observations are clearly on the higher end of the sale price scale. 

<u style="color: #f768a1">A Map of Average Price per Square Foot across Zip Codes</u>
- The following plot was created using [Holoviews](https://hvplot.pyviz.org/). 
- Choose a year in the drop down menu to analyze!
- Roll over the map to get more information about the price per square foot, zip code, borough and year! 

To give a spatial context to the distribution of average price per square foot across New York City, a choropleth map was created to identify where there was a clustering of more expensive apartments. Zip codes were used instead of boroughs to provide a more detailed depiction of this distribution across the city, but the borough information can still be accessed via the tooltip. 

<div id="DOF_priceByZIPCODE"></div>

There is a clear spatial clustering of higher prices in New York City. Prices have also been increasing overall from 2009 to 2015. Zip Code 11201 in Brooklyn is clearly getting darker over the years relative to its neighboring zip codes, showing an increase in price especially in that zip code in Brooklyn. Prices went up from $503/sqft in 2009 to $1076/sqft in 2015. 

## 2019 Sale Prices: Scrapping Craigslist 

As current sale prices were not available online, we decided that listings by real estate for sale by official brokers on [Craigslist](https://newyork.craigslist.org/search/reb?) would be a good proxy for current houses on sale. We thus decided to scrape 600 listings for each of the 5 NYC boroughs and compare the sale price to size for each listing. 

<u style="color: #f768a1">Sale Price to Size for each Listing on Craigslist</u>
- The following plot was created using [Altair](https://altair-viz.github.io).
- Use the legend to filter the scatterplot to a specific borough! 
- Zoom into the scatterplot to examine finer trends! 

Any listings that were priced at zero were removed. 

<div id="scraped_1_Scatter"></div>

2019 listings show that both Manhattan and Brooklyn are more costly at all sizes, and that most of the listings are smaller than the other boroughs. This is consistent with the trend in previous years as well. 

<u style="color: #f768a1">Choropleth Map of Average Price per Square Feet per Borough</u>
- The following plot was created using [Altair](https://altair-viz.github.io).
- Roll over the boroughs to get the name and average price per square feet of listings in that Borough!

<div id="scraped_2_MAP"></div>

The same trend as in previous the years is observed - Manhattan has the highest average price per square foot, with Brooklyn coming in second. Staten Island has prices slightly lower than Brooklyn. The Bronx and Queens have the lowest average price per square foot. 

## Conclusion 

Manhattan has always been the most expensive borough to live in in NYC, whilst it is the cheapest to stay in the Bronx and in Queens. There has been a small trend in increasing home sale prices in Brooklyn from 2009 to 2015 relative to the other boroughs. While taking note of this overall trend, it is also important to keep in mind that this is an aggregation of data over the boroughs, and different neighbourhoods within the boroughs could have different trends. 