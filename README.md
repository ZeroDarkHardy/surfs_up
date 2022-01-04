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

- A second analysis was performed on the weather data to include statistical information regarding the frequency and volume of rainfall on Oahu.  By comparing the data, we see that the average rainfall is significantly higher in December than it is in the month of June.  While the average temperature may still be favorable, we assume that far fewer people will be surfing and eating ice cream while it's raining. However, Oahu has a tropical climate, and rainfall often doesn't last long during the day. To provide our client with a more robust understanding of the conditions, we'll create histograms for the precipitation data and linear regression models to explore correlation between temperature and rainfall.

![linear_regression_gallery.png](https://github.com/ZeroDarkHardy/surfs_up/blob/main/resources/linear_regression_gallery.png)

- Our linear regression models suggest only a very slight correlation between temperature and rainfall.  While it does appear that there is a very subtle fall in the average rainfall as temperature increases, we see some of our highest rainfall values during what would otherwise be considered favorable temperatures.  Part of that could be because more instance of those common temperatures are observed, so let's take a look at a few histograms to see how frequently rain is observed in our client's business area:

![prcp_hist_gallery.png](https://github.com/ZeroDarkHardy/surfs_up/blob/main/resources/prcp_hist_gallery.png)

- Though Oahu has a tropical climate, with areas of rainforest, we can deduce from these histograms that it is NOT raining most of the time.  While the volume of rainfall is decently higher in December, the frequency of that rainfall seems to only marginally higher.

## Summary

- The data suggests that our client's business is a sound investment.  While it does rain harder and slightly more often in December, the average temperature stays optimal year round.  The additional rain will impact business in December, but if our predictive weather models stay accurate, the impact will be negligable.  It rains 195 days out of the year in Oahu, but usually only for brief periods during otherwise beautiful days.  If anything, brief tropical rain might actually help the clients business by pushing people into stores to wait while the rain passes, though our data provides no insight into this.