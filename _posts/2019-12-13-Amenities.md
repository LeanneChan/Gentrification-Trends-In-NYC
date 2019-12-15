---
title: "Dining and Nightlife Amenities"
date: 2019-04-13
published: true
tags: [dataviz, folium]
excerpt: "We used OSM data to analyze the locations of dining and nightlife amenities in New York City."
folium-loader:
  folium-chart-1: ["charts/amenities.html", "600"]
toc: true
toc_sticky: false
---

We used OSM data to analyze the locations of dining (cafes and restaurants) and nightlife (nightclubs and bars) amenities in New York City.

## Heatmap of Dining and Nightlife Amenities 

The following is a heatmap with 4 layers: neighborhoods, boroughs, dining amenities, and nightlife amenities. Users can toggle between the layers by pressing the button at the top right hand corner of the plot. It is clear that there are hardly any amenities on Staten Island, while amenities are concentrated all throughout Manhattan. Queens and Bronx have somewhat patchy clusters of amenities, while amenities are unevenly distributed across Brooklyn, with higher concentrations located closer to Manhattan. 

<div id="folium-chart-1"></div>

## Average Proximity to Amenities 

The following is an interactive application that allows users to specify an amenity and a value of 'n', to examine the average proximity of each node within the network to its n-th nearest amenity. This hence serves as a measure of accessibility to amenities, which we take to be a measure of gentrification. At n=1 (i.e. distance from the closest amenity), it is clear that Manhattan and the parts of Brooklyn closest to Manhattan are the most well-served by amenities, relative to the other boroughs. This disparity becomes even more evident where n=10 (i.e. distance from the tenth nearest amenity). 

<iframe src="https://serene-taiga-85680.herokuapp.com/Amenities_dashboard" height="1000" width="1000" frameBorder="0"></iframe>
