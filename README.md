# IBM Data Science

## Capstone project work for the IBM Data Science certification at Coursera

This project show an analysis of the publicly available [data set](https://data.iowa.gov/Sales-Distribution/Iowa-Liquor-Sales/m3tr-qhgy) on liquor retail sales in the state of Iowa, US. The goal is to try and predict the monthly sales per liquor type for a particular store based on information from historical sales and weather data. The work consists of few steps, briefly described as:

1. Exploratory data analysis:
  * Determine the data set attributes' type and range of allowed (or normal) values
  * Plot a few summarizing bar and line charts to become familiar with attributes' value distribution and relationship (correlation)
    * Notice the (expected) cyclic trend of the sales
  * Remove uninformative or not needed attributes (dimensionality reduction)
2. Transform the data:
  * Detemine the different sources of data (liquor sales come from the web site of the government of Iowa, weather information comes from NOAA's website
  * Merge the disparate sources
  * Generate new features
    * Lag values for the weather and sales parameters
3. Do (simple) machine learning:
  * The problem is simple univariate regression
  * Try: linear, lasso and ridge regression
  * Evaluate results on R^2 value
4. Summarize results
  * Models perform more or less the same
  * The evaluation period contains the outbreak of the COVID-19 pandemic and shows very interesting results (last plot in the notebook)
    * Total liquor retail sales in Iowa dropped for more than **90%** during this period!
    * R^2 values become negative because the model is simply not able to predict this (to be fair, neither was any of us :))!

For more information, check out the [report](https://github.com/popovstefan/IBM-Data-Science-Capstone-Project/blob/master/Capstone_Project_Report.pdf) and [presentation](https://github.com/popovstefan/IBM-Data-Science-Capstone-Project/blob/master/IBM_Data%20Science%20%40%20Coursera.pdf) files. For the actual code, take a look at the [Jupyter notebook](https://github.com/popovstefan/IBM-Data-Science-Capstone-Project/blob/master/Capstone_Project.ipynb).
