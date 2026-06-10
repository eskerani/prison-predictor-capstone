# Data cleaning plan 

* **Goal**: to make 5 disparate datasets compatible for simultaneous use with support vector regression (SVR).


## Incarceration 

* Make column names real
* Pivot longer
* Change state names so that they are not in all caps
* Rates will be calculated once joined with the other data, which includes population


## Crime

* Select state name, state abbreviation, year, population, violent crimes, and property crimes
* When there is not a state name associated with an observation, change the state name to ‘National’
* Rates will be calculated once joined with the other data


## Police spending
* Rename columns
* That’s it!


## Race
* Create a character-based race variable corresponding to the given race variable: 100 = white, anything else is non-white
* Group by the year, state code, and text race variable and calculate the sum of ASECWT
* Create a new column for non-white residents per 100k, calculated as (weight / summed weights) * 100,000
* Join the dataset with R’s built in FIPS codes dataset to get state names
* Select state name, year, race count, race sum
* Filter out values for white people


## Poverty
* Make column names real (based on 4th row) and delete rows 1-4
* Filter to get only the standard states included in the other datasets
* Loop through the data to impute years


## All
* Join based on state and year
* Filter for years 1980-2020
* Calculate rates per 100k for poverty, incarceration, crime (either number/population * 100k or poverty percent * 100k)


## For SVR
* Standardize all measures using standard_scaler
* Create a new column corresponding to national incarceration rate for a given year, filter out national rates for all other measures
* Each variable will be broken out and used in its own model after the train/test split
