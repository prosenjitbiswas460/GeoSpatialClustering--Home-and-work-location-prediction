# GeoSpatialClustering

The idea of this project is to analyse and cluster locations of a driver and tag them as home, work and secondary work and non work locations. This analysis will enable us to understand the driver behaviour and work patterns thereby, optimizing work hours and pointing out anomalous behaviour. The data used is arbitrary and the GPS coordinates are randomly sampled from NYC taxi trajectory dataset. The data used is also uploaded in the repo. The project is written in an object oriented way with Python; while the map visualizations are done with the help of a python library called 'Folium'. The advantage with this library is that we do not need shape files as with some other geolocation based libraries. Among the folium maps, first one is a dynamic heatmap of traffic, second is a timed heat map that shows the points where the traffic was seen with time, third is a clustered map with pointers denoting each cluster on the map.
1. Unfortunately the folium maps do not seem to render on GitHub natively.It likely has something to do with the site's settings on running JavaScript. However, we should be able to drop the github link to the .ipynb file into nbviewer.org and get a full dynamic output, when provided a valid folium.Map instance. Please follow the below link:
https://nbviewer.jupyter.org/

2. The dynamic plotly content is also not rendered properly on github. We can look at the plots after converting them into static content with fig.show("png") in the respective functions. Doing so, crams up the plots and makes them poor to look at. For better understanding, please remove the argument "png" from fig.show("png") at all the places.

The end result for this data set is a set of clustered data points plotted on maps with the help of algorithms like KMeans, DBscan and deep learning based self organizing maps (SOM). The evaluation metrics and conclusion is included as well.

Best Experience: please download or clone the ipynb file and use the dynamic content to view the maps and analysis.
