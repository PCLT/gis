Quick analysis of wages and sexual orientation using US Census [PUMS data](https://www.census.gov/programs-surveys/acs/data/pums.html)

- **data-munging**: merging data from 2014-2016, at household and population levels
- **download**: download PUMS shapefiles
- **merge_pums**: merging shapefiles
- **models**: basic OLS at country level, state level, and simple geographically weighted regression
- **mapping**: using geopandas to map results

Notable Findings
- across the country, people in same-sex marriage earn 9% more on average (controlling for race, age, sex, education level, household language)
- this difference varies substantially at state levels
- geographically weighted regression (GWR), which allows the parameters of the regression to vary spatially shows that the association between sexual orientation and wages varies substantially geographically
- patterns for men and women are also very different.  Generally women in same-sex marriages earn more than their opposite-marriage counterparts.  This is somewhat reversed for men.


Limitations:
- analysis only looks at married couples (same-sex vs. opposite-sex).  Findings might not extrapolate to unmarried people
- ignored those who have self-selected out of employment
- did not control for chosen profession or other sources of income!
