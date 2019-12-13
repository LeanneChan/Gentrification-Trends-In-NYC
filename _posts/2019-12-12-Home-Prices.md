---
title: "Home Sale Price Trends"
date: 2019-12-12
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Viz on craigslist prices and Department of Finance Data."
altair-loader:
  scraped_1_Scatter: "charts/plot1_craigslistPrices.json"
  scraped_2_MAP: "charts/plot2_craigslist_PricebyBorough.json"
  DOF_priceByBorough: "charts/plot3_prices_0915.json"
hv-loader:
  DOF_priceByZIPCODE: "charts/plot5_priceZipCode.html"
toc: true
toc_sticky: false
---

This post will show examples of embedding interactive charts produced using [Altair](https://altair-viz.github.io) and [Hvplot](https://hvplot.pyviz.org/).

## Current For Sale Prices by Scrapping Craigslist

Below is an interactive scatter plot of price to size of homes for sale across different NYC boroughs in 2019 (based on current Craigslist listings). Click on the legend to view data on specific boroughs! 


<div id="scraped_1_Scatter" style="width:2px; height: 500px;"></div>


### More Craigslist 2 

<h3 style="color:yellow;"> Plot of Average Price Per Square Foot by Borough </h3>
<div id="scraped_2_MAP"></div>

## Department of Finance Data 
Past data was downloaded from the [Department of Finance]("https://data.cityofnewyork.us/City-Government/NYC-Citywide-Annualized-Calendar-Sales-Update/w2pb-icbu") and plotted. 


### Plot 1: Comparison of AveragePrice per Square Foot across boroughs, 2009-2015. 
<div id="DOF_priceByBorough"></div>

### Plot 2: Hexbin Facetgrid comparing Price of Housing to Size per borough over years. 
![Hexbin FacetGrid]({{site.url}}{{site.baseurl}}/assets/images/plot4_Size_to_price_ByBoroughYear.png)


### Plot 3: Map Average Price per Sqaure Foot across Zip Codes 2009-2015
<div id="DOF_priceByZIPCODE"></div>


## GIF Construction Permits 1989-2019
![GIF]({{site.url}}{{site.baseurl}}/assets/images/permits_89_19.gif)

## Notes

- See the [raw source code](https://raw.githubusercontent.com/nickhand/static-site-template/master/_posts/2019-04-13-measles-charts.md) of this post for details on how these charts were embedded.
- See the [week 13 lecture slides](https://github.com/MUSA-620-Fall-2019/week-13/blob/master/lecture-13.ipynb) for the code that produced these plots.

**Important: When embedding charts, you will likely need to adjust the width/height of the charts before embedding them in the page so they fit nicely when embedded.**
