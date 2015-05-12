# Where are the Starbuck's at?
There are fewer Starbuck's locations near census tracts with high poverty rates
than those with low rates, according to analysis in this project. The average number
of Starbuck's per 1,000 population per square mile in census tracts with high
poverty is 0.18 (95% CI [0.14, 0.23]) and in census tracts with low poverty
is 0.32 (95% CI [0.31, 0.34]).

These two rates were found to be statistically significant with over 95%
confidence using Monte Carlo sampling to perform a permutation test. The
confidence intervals were found similarly using bootstraping.

## Data
### Sources
Census data were compiled and downloaded on [Social Explorer](http://www.socialexplorer.com).
Shapefiles were acquired from the [County of Los Angeles' Open Data Portal](https://data.lacounty.gov/Geospatial/Census-Tracts-2010/ay2y-b9rg).
Locations of Starbucks were found using the [Google's Places API](https://developers.google.com/places/webservice/) using Radar Searches. The dataset of locations is cached in the folder `cached_data`.

### Locations in Repo
There are three directories in this repo that have data:

* `los_angeles` has the shapefiles for Los Angeles County
* `census_data` has the original census data csv files
* `cached_data` has several RData dumps that hold data that took a substantial
  amount of time to process. The original code used to acquire and process all
  this data can be found in the Analysis.Rmd file, with much of it commented
  out.