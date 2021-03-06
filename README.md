# What-if Analysis of Residential Real Estate in New Jersey

## Summary
Real estate valuation depends on a number of factors. More often than not, an individual assesses four important factors while investing on a residential real estate. These are: school rating, crime, mass transit and population. The aim of the project is to examine the impact of these 4 metrices affecting valuation of residential real estate of New Jersey and thereby identify counties that are best to live. 

### Note
Since, real estate data could not be obtained for South of New Jersey, hence the analyses is restricted to 11 counties. As per a report every household in NJ has an average of 2.5 members per family, hence analysis was limited to residences with 3 bedrooms.

## Team members
Harmeet Kaur, Nitin Sharma, Deborah Ofsievich, Jean Pino 

## Installation packages and libraries used
Jupyter notebook, Python, Pandas, Matplotlib, NumPy, SciPy

## To run  
* To get a copy of the project up and running on your local machine for development and testing purposes, clone the repo, launch jupyter notebook and run the ipynb files 
* API keys will have to be obtained for google map and schooldigger


## Data Source
* School data: [Schooldigger](https://www.schooldigger.com/)
* Crime data: [NJ State Police](https://www.njsp.org/)
* Real-estate data: [NJMLS](https://www.newjerseymls.com/)
* Transit: [NJ Transit](https://www.njtransit.com/hp/hp_servlet.srv?hdnPageAction=HomePageTo)
* Population: [United States Census Bureau](http://www.census.gov/)

## Methodology
For this data were retrieved from different sources: API calls were made to retrieve school data from schooldigger.com, crime records from NJSP.Gov, residential real estate data from newjerseymls.com, mass transit information from NJ Transit (API) and population of counties from United States Census Bureau. Isolated data relevant for the project from each data source, cleaned and transformed each dataset. A master dataframe was created by merging all the data using pandas.

![method](https://github.com/Harmeet2504/Project-What-if-analysis-of-residential-real-estate/blob/master/Screen%20Shot%202020-02-22%20at%208.26.24%20AM.png)

Correlation between the metics were measured in terms of Pierson's Coefficient of correlation. Trend/ relationship was examined by generating regression equation from scatter plots. Percentage of population versus crime of each counties were compared by generating donut plots(variant of pie plot). Bins were created to designate areas with high , moderate, low crime rates.  School data per county was analysed by generating stacked bar plots. NJ transit map was generated using google map and markers were used for indicating each station.
Following are a few images from the analyses:

* School versus residential price

![School Versus Residential Price](https://github.com/Harmeet2504/Project-What-if-analysis-of-residential-real-estate/blob/master/input-code-output-files/output_files/Figures/Average%20School%20Score%20Versus%20Average%20Resident%20Price.png)

* Percent crime per county

![Crime per county](https://github.com/Harmeet2504/Project-What-if-analysis-of-residential-real-estate/blob/master/input-code-output-files/output_files/Figures/Percent_Crime_Per_County.png)

* Crime rate versus school score

![](https://github.com/Harmeet2504/Project-What-if-analysis-of-residential-real-estate/blob/master/input-code-output-files/output_files/Figures/Crime%20Rate%20vs%20School%20Score.png)

* Residntial price in best counties 

![](https://github.com/Harmeet2504/Project-What-if-analysis-of-residential-real-estate/blob/master/input-code-output-files/output_files/Figures/Residntial_price_in_best_counties_of_NJ.png)

## Findings
* Counties with good schools have high residential valuation.
* Mass transit affects both residential price as well as crime of an area.
* Bergen, Monmouth, Morris are amongst the best counties to live observed from the analysis
* No clear correlation was observed between crime and residential price as population of an area tend to affect the overall crime rate.
* There are many other factors that affect residential valuation which could not be covered in the project. Taking them into consideration and anlayzing them holistically will provide greater insights into the dynamics of residential property valuation.

## Challenges
* API call made to retrieve records from  multiple pages. For loops used to deal with pagination and data unpacking.
* One Station was tagged to multiple Stations. Had data for Light rails and path. Data was transfor,ed and cleaned to remove ambiguity
* No real estate data could be retrieved for south of New Jersey. Hence, the study is limited to observations from North Jersey.






