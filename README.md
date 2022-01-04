# surfs_up
---
## Overview of Project

Our client is interested in opening a hybrid surf shop/ice cream parlor on the the island of Oahu.  Since both of the the store's primary products' sales are likely dependent on favorable weather conditions, the client has asked us to analyze a sample of of historical weather data to determine the business' viability.  Using the provided SQLite database containing the weather data, we will perform statistical analysis to determine the fluctuations in conditions between extremes, comparing the months of June and December.

## Results

![deliverable1-2.png](https://github.com/ZeroDarkHardy/surfs_up/blob/main/resources/deliverable1-2.png)

- The first thing we did was aggregate and temperature data for the two months, and obtain the descriptive statistics.  On their face, this produces an immediately promising outlook for our client's prospective business.  If we assume that people only buy ice cream on warm days, and define a warm day as above 70° fahrenheit, then our data suggests that the average temperature (74.9° in June, 71° in December) will be warm year round, though the bottom quartile of data from December falls slightly below that metric.

![histogram_gallery.png](https://github.com/ZeroDarkHardy/surfs_up/blob/main/resources/histogram_gallery.png)

- We created histograms for the temperature data from the two months, to make sure our averages are dependable and to see what the most commonly observed temperatures were.  Again, this produced promising data, showing the highest frequency of observed temperatures were north of our margin for favorable temperatures.  However, our client is rightly concerned that rainfall (or the absence thereof) may play an important factor in the store's constancy of sales...

![stats_gallery.png](https://github.com/ZeroDarkHardy/surfs_up/blob/main/resources/stats_gallery.png)

- A second analysis was performed on the 

![linear_regression_gallery.png](https://github.com/ZeroDarkHardy/surfs_up/blob/main/resources/linear_regression_gallery.png)

## Summary