---
title: "3 Decades of Construction Permits in NYC"
date: 2019-12-13 
published: true
tags: [dask, big data]
excerpt: "3 Million Points, 1 GIF"
toc: true
toc_sticky: false
---

## A GIF of Construction Permits 1989-2019 in New York City 

A rise in construction permits is a good indicator of gentrification as areas under gentrification are likely to see a spike in renovations and the construction of new buildings. Data was taken from the [Department of Buildings](https://data.cityofnewyork.us/Housing-Development/DOB-Permit-Issuance/ipu4-2q9a). Given the large dataset of 3.62Million points, [Dask](https://dask.org/) was used to load the data and [Datashader](https://datashader.org/) was subsequently used to create a map of points of permits for each year from 1989-2019. 

![GIF]({{site.url}}{{site.baseurl}}/assets/images/permits_89_19.gif)

It is unclear if data for 1989 is an accurate representation of all construction permits, thus more research must be done to determine if construction was only concentrated around Queens. Over the past 30 years, construction has always been concentrated in Manhattan, but there is a clear trend of there being more construction in Brooklyn, especially the area closer to the East River. This could be because waterside developments are of demand. The proximity to Manhattan also makes the area a favorable site for workers to live in and commute into Manhattan. 
