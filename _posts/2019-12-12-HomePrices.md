---
title: "Home Sale Price Trends in New York"
date: 2019-12-12
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Viz on craigslist prices and Department of Finance Data."
altair-loader:
  scraped_1_Scatter: "charts/plot1_craigslistPrices.json"
  scraped_2_MAP: "charts/plot2_craigslist_PricebyBorough.json"
  DOF_priceByBorough: "charts/plot3_prices_0915.json"
hv-loader:
  DOF_priceByZIPCODe: "charts/plot5_priceZipCode.html"
toc: true
toc_sticky: true
---

This post will show examples of embedding interactive charts produced using [Altair](https://altair-viz.github.io) and [Hvplot](https://hvplot.pyviz.org/).

## Current For Sale Prices by Scrapping Craigslist

Below is an interactive scatter plot of price to size of homes for sale across different NYC boroughs in 2019 (based on current Craigslist listings). Click on the legend to view data on specific boroughs! 


<div id="scraped_1_Scatter" style="width:2px; height: 500px"></div>

```python
import altair as alt
alt.renderers.enable('notebook')
```

<h1> "Plot or Average Price Per Square Foot by Borough </h1>
<div id="scraped_2_MAP"></div>

## Holoviews Example

Lastly, the measles incidence produced using the Holoviews package:

<div id="hv-chart-1"></div>

## Notes

- See the [raw source code](https://raw.githubusercontent.com/nickhand/static-site-template/master/_posts/2019-04-13-measles-charts.md) of this post for details on how these charts were embedded.
- See the [week 13 lecture slides](https://github.com/MUSA-620-Fall-2019/week-13/blob/master/lecture-13.ipynb) for the code that produced these plots.

**Important: When embedding charts, you will likely need to adjust the width/height of the charts before embedding them in the page so they fit nicely when embedded.**
