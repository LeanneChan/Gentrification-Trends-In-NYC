---
title: "Socio-Economic Trends in New York City"
date: 2019-12-13
published: true
tags: [dataviz, altair]
excerpt: "We compared census tract information for years 2009 and 2017 to examine socio-economic trends in New York City. "
altair loader: 
  altair-chart-1: "charts/MedianIncome.json"
  altair-chart-2: "charts/PctPoverty.json"
  altair-chart-3: "charts/PctWhite.json"
toc: true
toc_sticky: false
---

# Median Household Income

The following is an interactive chart comparing median income of households in 2009 and 2017. Tracts with no change in median income are reflected along the diagonal axis running from bottom left to top right of the plot; tracts that experienced increase in median income between 2009 and 2017 (possibly indicative of gentrification) are represented above this diagonal axis, while tracts that experienced a decrease in median income are represented below the diagonal axis. The shading of the plot indicates how many tracts (across New York City) belong within each category. 

It is clear at first glance that most tracts remained between either the $0 - $50,000 or $50,000 - $100,000 brackets and did not experience major improvements in median income between 2009-2017, as evident from the dark blue shading and large circles within those boxes along the diagonal axis. Interestingly, a significant number of tracts progressed from the $0 - $50,000 bracket to the $50,000 - $100,000 bracket between 2009-2017, as reflected by the turqoise box above the diagonal axis and the mid-sized circle within. 

Clicking on the bar chart allows the user to filter census tracts by borough, to see how tracts within each borough fared between the 2 years. The number of tracts within each category is represented by the size of circles. Manhattan has experienced the most gentrification, since most boxes above the diagonal axis contain circles of varying sizes, implying that many census tracts have experienced a significant increase in median income between 2009-2017. In contrast, Bronx has experienced only a little gentrification, since only 2 boxes above the diagonal axis contain some relatively small circles.

<div id="altair-chart-1"></div>

## Percentage Living Below 100% 

<div id="altair-chart-2"></div>

## Percentage White Population

<div id="altair-chart-3"></div>

