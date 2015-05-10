# Franchise Distributions
Will Jones  
April 1, 2015  



This project examines correlations between the number of Starbuck's locations
in an area with demographics information---such as ethnic makeup, median income,
poverty level. For the locations, this project examines census tracts in Los
Angeles County.

Census data is provided by the 2010 census for estimates of population and
ethnic makeup, while we use ACS five-year estimates for median income and
poverty level.



Here are some histograms of the basic demographic data:

![](Analysis_files/figure-html/unnamed-chunk-3-1.png) 







Now that we have a selection of census tracts to examine, we need to find how
many Starbucks locations are nearby each. To get all the relevant locations in
the area, we can do a series of searches on Google around specially chosen
points. We can do this with 24 radar searches with radii of 13 kilometers. The
maximum radius is 50km, but this increases the likelihood that we will miss
locations, for the API call only returns up to 200 locations at once.(The
function here to draw circles was adapted from code written by
Gregoire Vincke, in a 
[Stack Overflow answer](http://stackoverflow.com/a/29133886/4645559).)
![](Analysis_files/figure-html/unnamed-chunk-5-1.png) 



![](Analysis_files/figure-html/unnamed-chunk-6-1.png) 

Notice there are some areas with no locations. To the north is Angeles National
Forest, and the western stretch is Santa Monica Mountains Recreational Area. In
some areas, that are likely less populated, the locations seem to align with
whatever freeways are nearby.

Now we need to calculate how many Starbuck's locations are near each census
tract.

![](Analysis_files/figure-html/unnamed-chunk-7-1.png) 

TO DO:

* Get Histogram of starbucks
* Determine distribution of Starbucks
* For each variable, do Monte Carlo simlulation to determine whether they are
  correlated. Make each variable into a categorical variable.



