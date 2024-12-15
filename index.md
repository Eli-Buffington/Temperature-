---
layout: default
---
## Correlation between carbon dioxide  emissions and Temperature in the United States


# Introduction

Climate change has irrefutable evidence for its existence. The research has been conducted on datasets going back hundreds of years, showing an increase in the global temperature that is undeniable, giving the length and accuracy of the data. But the relatively lax carbon dioxide regulations and tracking, where corporations have every economic desire to try to circumvent, are much of what is reported when it comes to carbon dioxide emissions. Do these guidelines help predict the change in temperature? If so, how long before the effects are statistically significant, as climate is notoriously unpredictable past a few days. 
Is there a correlation between a change in carbon dioxide emissions and a change in  Temperature? We suspect a correlation because of a multitude of peer reviewed studies on the effect of greenhouse gasses and climate change, but would a statistically significant correlation show up in the relatively short 25-30 years of our data? 
 The data that we used was temperature data from the United States and carbon dioxide data from the United States from 1991 to 2019. These were two separate datasets, which were merged together for further analysis. The data was from reputable sources and thus was very easy to process, leading to few issues with the data. Downloading the data was made simple by the websites allowing a choice between different time periods and sample frequencies. The only slight hurtle was lining up the data and merging the two dataframes together, as the columns, while both being a date, were formatted differently, leading to significant reprocessing before merging. 

We graphed the merged data frame on the same graph and attempted to line the effects of carbon dioxide emissions up with a corresponding effect on temperature. We then regressed the change in carbon dioxide emissions on the change in temperature, both shifted and unshifted, to find the correlation between these two datasets by obtaining a p-value and a line of best fit. 


# Methods & Results

We compared these two time series datasets by merging the two separate data frames together on the time column. We only used yearly data averaged on January 1st of every year. One of the bigger issues that came up was how to plot data with two different units on the same graph. The way we solved this is by having two different y-axes, one on the left and one on the right side of the graph, so that we could see both graphs together on the same chart. 

