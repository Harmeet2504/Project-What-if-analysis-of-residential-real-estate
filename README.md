# Project-What-if-analysis-of-residential-real-estate
The aim of the project is to examine the impact of 4 metrices (school rating, crime, mass transit, population) affecting valuation of  residential real estate of NJ.

# Data Source
* School data: [Schooldigger](https://www.schooldigger.com/)
* Crime data: NJSP.Gov
* Real-estate data: newjerseymls.com
* Transit: NJ Transit
* Population: United States Census Bureau

# Methodology
![method](https://github.com/Harmeet2504/Project-What-if-analysis-of-residential-real-estate/blob/master/Screen%20Shot%202020-02-22%20at%208.26.24%20AM.png)

For this data were retrieved from different sources: API calls were made to retrieve school data from schooldigger.com, crime records from NJSP.Gov, rresidential real estate data from newjerseymls.com, mass transit information from NJ Transit (API) and population of counties from United States Census Bureau.

A master dataframe was created by merging all the data using pandas and correlation between the metics were measured in terms of Pierson's Coefficient of correlation. Linear relationship was examined by generating linear regression equation from scatter plots.Percentage of population versus crime of each counties were compared by generating donut plots(variant of pie plot). School data per county was analysed by generating stacked bar plots.NJ transit map was generated using gmap. All codes were written in python and pandas using different modules like matplotlib, statistical analysis was done using numpy and scipy.

![alt-text-1](image1.png "title-1") ![alt-text-2](image2.png "title-2")

# Installation packages and libraries used
Jupyter notebook, python, pandas, matplotlib




