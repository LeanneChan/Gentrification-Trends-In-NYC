---
title: "Taxi Pickups and Dropoffs"
date: 2019-12-13
published: true
tags: [dataviz, hvplot, holoviews]
excerpt: "We examined taxi pickups and dropoffs in New York City between January and June 2019, focusing specifically on rides between 5pm on Friday evening to 5am on Monday morning, to analyze where leisure activities are concentrated in the City."
hv-loader:
  hv-chart-1: "charts/DropoffsHour.html"
  hv-chart-2: "charts/DropoffsNeighborhood.html"
  hv-chart-3: "charts/PickupsHour.html"
  hv-chart-4: "charts/PickupsNeighborhood.html"
toc: true
toc_sticky: false
---

We examined taxi pickups and dropoffs in New York City between January and June 2019 to analyze where people spend their leisure time. We filtered out specifically rides that occurred between 5pm on Friday evening to 5am on Monday morning, under the assumption that people participate in leisure activities during this time period, and that taxi rides are representative proxies of where such activities are located.  

## Yellow Cab Dropoffs

The following is an interactive plot reflecting the number of pickups in each borough at various hours of the day. It is extremely clear that Manhattan (shaded in red) experiences the highest human traffic at all times of day, for the time period examined. It is followed by Queens, and then Brooklyn, suggesting that leisure activities conducted on weekends are congregated in these boroughs. 

<div id="hv-chart-1"></div>


The density of taxi dropoffs (and by extension leisure activities) between 5pm on Friday evening and 5am on Monday morning is also evident from the following plot, where most of Manhattan is lit in green, indicating high numbers of taxi dropoffs relative to the rest of the plot, colored in purple. The only exception is a tract in Queens, which is shaded in blue (located at the bottom right corner of the map): this is the tract containing JFK airport, thereby explaining the unusual density of taxi dropoffs. 

<div id="hv-chart-2"></div>

## Yellow Cab Pickups

Similar plots were made for taxi pickups, which reflect similar trends as described above. 

<div id="hv-chart-3"></div>

The tract in Queens containing JFK airport is shaded in bright green in this map, suggesting that it experiences much higher volume of pickups relative to the rest of New York City as compared to the volume of dropoffs.

<div id="hv-chart-4"></div>
