# Where are the Starbuck's at?
There are more Starbuck's locations near census tracts with high poverty rates
than those with low rates, according to analysis in this project. There are
about 1.28 (95% CI [0.99,1.63]) Starbuck's per 1000 people near census tracts
with over 40% of their residents living below the poverty level, while there
are only 1.02 (95% CI [0.98,1.06]) Starbuck's per 1000 people near census tracts
with lower rates of poverty.

These two rates were found to be statistically significant with over 95%
confidence using Monte Carlo sampling to perform a permutation test. The
confidence intervals were found similarly using bootstraping.

## Data
### Sources
Census data was acquired from SocialExplorer.com.
Shapefiles were acquired from ___
Locations of Starbucks were found using the Google Places API using Radar
Searches. The dataset of locations is cached in the folder `cached_data`.

### Locations in Repo
There are three directories in this repo that have data:

* `los_angeles` has the shapefiles for Los Angeles County
* `census_data` has the original census data csv files
* `cached_data` has several RData dumps that hold data that took a substantial
  amount of time to process. The original code used to acquire and process all
  this data can be found in the Analysis.Rmd file, with much of it commented
  out.