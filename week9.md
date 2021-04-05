# Using Visualizations to Monitor Changes and Harvest Insights from a Global-Scale Logging Infrastructure at Twitter

![image](https://github.com/mike3osei/reflections-1/blob/master/img/week9.png) 

This publication describes one of Twitter's largest datasets in their organization. This visualization is a unified logging infastructure that showcases user events across all their clients (mobile, web, etc.). They focus on monitoring and exploring a large collection of log events as well as how they go about performing analysis at scale. 

## Link
https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7042487


## Initial Response

Intitially I found it very intersting how Twitter had been collecting data in their "Hadoop" data warehouse, but due to its slowness they wanted to build a whole new infastructure to perform analysis much faster. It was interesting to see that previously they utilized some open source software like MapReduce to make things easier previously but resulted on restructuring their data culture in order to take away better insights. I found it neat that no matter how big of the dataset they had everything was pretty much a tree in some way at the end of the day. I enjoyed how they went through A/B testing to figure out how users could also intertact with this data vis more efficiently instead of having to know for instance the six-part event names that define the hierarchy or domain they are interested in.

## Takeaways

I thought it was interesting how they chose to represent event volumes using color in the data vis. I honestly think this was the only like bad part in terms of like accessibility. You would think there would be another like variant to solidify that color and something something else was used to showcase that metric. For example using color and shape but it was pretty much just color variances that showcased the event volumes. I also did take away their testing approach when it came to improving the UX involved in datavis. I found that interesting how they were able to leverage that space to improve the quality of this data visualation.