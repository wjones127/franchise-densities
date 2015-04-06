# Density of Franchises
There are over 14,000 McDonald's restaruants in the U.S. This brings up the interesting question about where these are placed? Are they equally spaced throughout the nation? Or are there interested correlations between the density of these restaraunts in a region and demographic factors like median income or even the racial composition of the local population?
These questions don't just apply to McDonald's; Starbuck's, Taco Bell, Target and many other companies have a similarly large number of widely distributed locations in the U.S.
This project will look into these questions, examining connections between demographics of areas and the concentration of locations of particular frachises. The end result will be a web application that allows visitors to explore these relationship graphically.

## Data
*Google Places API* will provide the locations of these franchises. The docs for this API can be found [here](https://developers.google.com/places/webservice/search).
*Census* data will be used to determine demographics factors.


## Variables
- `longitude` and `lattitude` of locations, provided by Google API
- `census.tract`: this will be the unit of observation. The locations will need to be binned into these, which may be a complex process.
- `median.income`: median income of the census tract
- `population`: population of a census tract
- `prop.white`, `prop.black`, `prop.asian`, etc.: proportion of census tract that is of a particular race
- Other variables could also be included that are tied to census tracts.


## End Product
The end product will be a web application displaying some exploratory analysis for a particular franchise. While it would be cool and theoretically posible to allow for the user to input an arbitrary restaurant, there probably is no efficient way to do the necessary calculations on the fly, especially the part where we need to bin the locations into census tracts. Thus, the best we can do is have a list of franchises for which there is data that has already been calculations done.

