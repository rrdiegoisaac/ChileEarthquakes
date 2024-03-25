# ChileEarthquakes
An analysis of earthquakes in Chile between 2012 and 2024

##### data source https://evtdb.csn.uchile.cl

### Cleaning Data
The db doesn't contain null data

![image](https://github.com/rrdiegoisaac/ChileEarthquakes/assets/164385592/f5c9d190-18d5-449b-8fef-db836429acfb)

However, it contains a time series that was imported as object, so it must be changed to dt
![image](https://github.com/rrdiegoisaac/ChileEarthquakes/assets/164385592/6f90b5d9-7f54-4819-b4b8-fe321661b18b)

### EDA

The data frequency appears to exhibit anomalies at the extremes, attributed to the limited amount of data available. However, for the remaining years, the distribution appears to align more closely with expected norms

![correlation](assets-img/earthquakesfrecuency.png)

If we examine the distribution of earthquake magnitudes, it becomes apparent that the vast majority of data falls within the range of 4 to 5 degrees. The most frequent occurrence is that of 4 degrees, which appears 290 times
![correlation](assets-img/earthquakesdistribution.png)

When examining the distribution of magnitude over time compared to depth, a certain level of typicality is observed in the data. Thus, at first glance, there appears to be no strong correlation between depth and earthquake magnitude
![correlation](assets-img/magnitudeovertime.png)

Upon conducting a Pearson correlation, the coefficient 'r' between magnitude and depth is found to be 0.20. This outcome aligns with expectations following the observation of the magnitude-depth plot over time
![correlation](assets-img/correlation.png)

Upon generating a density map to visualize occurrences of depth in conjunction with magnitude, it is evident that the majority of events cluster around an approximate depth of 50 kilometers. The data exhibits a typical pattern
![correlation](assets-img/densityheatmap.png)


When observing earthquake occurrences on a geographic map, there does not appear to be any particular regions in Chile where earthquakes are more predominant, except for the southernmost part of the country where fewer significant occurrences are noted
![correlation](assets-img/scatter_mapbox.png)


