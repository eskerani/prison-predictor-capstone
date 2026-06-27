# Schema

<img width="661" height="321" alt="image" src="https://github.com/user-attachments/assets/ca414549-2b70-4b4c-bd62-d2ddbeb1433f" />

This generally represents how five disparate datasets will be joined together, though rather than using an observation ID the datasets will be joined based directly on the year and state of a given observation. Once joined, rates per 100,000 will be calculated based on the population information present in the poverty dataset. The combined and cleaned data will contain the columns below: 

| Column name        | Description                                                                                                                              | Type  | Units                              |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------|-------|------------------------------------|
| State              | The state which an observation corresponds to                                                                                            | str   | NA                                 |
| year               | The year an observation corresponds to                                                                                                   | int   | years                              |
| tot_pop            | The total population in a given state/year                                                                                               | int   | People                             |
| incar_rate         | The number of people incarcerated per 100,000 people in a state/year                                                                     | float | People per 100,000                 |
| tot_crime_rate     | The total number of recorded crimes per 100,000 people in a state/year                                                                   | float | Crimes per 100,000 people          |
| violent_crime_rate | The number of recorded violent crimes (comprised of homicide, rape, robbery, and aggravated assault)  per 100,000 people in a state/year | float | Violent crimes per 100,00 people   |
| prop_crime_rate    | The number of recorded property crimes (comprised of burglary, larceny, and motor vehicle theft) per 100,000 people in a state/year      | float | Property crimes per 100,000 people |
| pov_rate           | The number of people in poverty per 100,000 in a state/year                                                                              | float | People per 100,000                 |
| non_white_rate     | The number of people who identify as anything other than white per 100,000 in a state/year                                               | float | People per 100,000                 |
| spending_rate      | The number of dollars spent by state and local governments on police per 100,000 people in a state/year                                  | int   | Dollars spent per 100,000 people   |
