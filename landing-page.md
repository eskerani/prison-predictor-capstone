# Welcome to the landing page for *Crime and What Else? Investigating the Predictive Power of Social Factors on Incarceration Rates*
(A capstone project completed by Emery Kerani)

This project seeks to explore associations between social factors and national incarceration rates, in order to investigate whether crime or other variables (e.g. racial diversity)
are better predictors of the national incarceration rate across time. 

If you would like to explore the past deliverables for this project, they can be found in the following folders:
* [Milestone 1/Project Proposal](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M1-proposal)
* [Milestone 2/Data Summary](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M2-data-summary)
* [Milestone 3/Draft Poster](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M3-poster-draft)
* [Milestone 4/Draft Writeup](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M4-writeup-draft)
* [Milestone 5/Final Deliverables](https://github.com/eskerani/prison-predictor-capstone/tree/main/deliverables/M5-final) (*Currently in progress*)

If you would like to investigate the data or cleaning process, navigate to the [data folder](https://github.com/eskerani/prison-predictor-capstone/tree/main/data). 
Raw data is contained in the `raw` folder; preliminary findings/EDA are in the `interim` folder; and the final combined dataset and script used to clean it are in the `processed` folder.

### Visualizations
The visualizations used on the poster are reproduced here, in case you would like a closer look:

<img width="1176" height="1176" alt="capstone data sketch drawio" src="https://github.com/user-attachments/assets/b52e4b0b-382d-4c7d-b6f5-d2ccd428b37c" />

*Figure 1: A diagram of the pipeline used for this project, from ingestion to modeling*

---

<img width="1844" height="1499" alt="all_graph" src="https://github.com/user-attachments/assets/4c8df799-35ff-41c1-86ee-3b2364cfc189" />

*Figure 2: A time series graph displaying the national incarceration rate compared to SVR predictions based on police spending data only (green dotted) and all features (orange dashed)*

---

<img width="2249" height="1500" alt="rmse_graph" src="https://github.com/user-attachments/assets/e2a6c868-657c-4c62-a9d2-e84bb873e1e0" />

*Figure 3: A bar plot depicting the RMSEs of all models for comparison*

---

<img width="2230" height="933" alt="poster_table" src="https://github.com/user-attachments/assets/418f9e6c-f55b-4e35-b8ab-0af392fa2999" />

*Table 1: A table displaying the results and stats for all models/variables. The best results are highlighted in darker purple, with worse results in lighter shades*

---

### Full data citations
1. Bureau of Justice Statistics. Corrections Statistical Analysis Tool [dataset]. n.d. https://csat.bjs.ojp.gov/advanced-query
2. Sarah Flood, Miriam King, Renae Rodgers, Steven Ruggles, J. Robert Warren, Daniel Backman, Etienne Breton, Grace Cooper, Julia A. Rivera Drew, Stephanie Richards, David Van Riper, and Kari C.W. Williams. IPUMS CPS: Version 13.0 [dataset]. Minneapolis, MN: IPUMS. 2025. https://doi.org/10.18128/D030.V13.0
3. Federal Bureau of Investigation. Summary Reporting System [dataset]. 2025. https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads
4. United States Census Bureau. Annual Survey of State and Local Government Finances [dataset]. 2026. Published by Nikhita Airi, Lucy Dadayan, Gabriella Garriga, and Kim Rueben at the Urban Institute. https://state-local-finance-data.taxpolicycenter.org/pages.cfm
5. United States Census Bureau. Number of Poor and Poverty Rate by State [dataset]. 2025. https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-poverty-people.html
