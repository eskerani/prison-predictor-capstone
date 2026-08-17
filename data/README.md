# `data/`

Project data lives here. The repo root `.gitignore` excludes large or sensitive subfolders by default. The structure below is the convention you should follow.

```
data/
  raw/         # original inputs, never edited in place        (gitignored)
  external/    # third-party data you did not generate         (gitignored)
  interim/     # intermediate scratch outputs                  (gitignored)
  processed/   # cleaned, analysis-ready snapshots (committable if small)
  README.md    # describe each dataset: source, license, date, size
  SCHEMA.md    # describe processed dataset schemas once they stabilize
```

## What to **always** commit

- This `README.md` describing every dataset, with: source URL or contact, license, date pulled, approximate size, who in the team owns it, and any ethics / consent notes.
- A `SCHEMA.md` documenting the columns, types, and units of your processed datasets, once they stabilize.
- Small (< 1 MB) reproducible processed snapshots under `data/processed/` if your analysis depends on a specific version.

## What to **never** commit

- Personally identifiable information (PII), protected health information (PHI), or any data subject to a data use agreement that forbids redistribution.
- Credentials, API keys, OAuth tokens, or `.env` files.
- Multi-megabyte raw downloads. Document how to fetch them in this README instead.

## Dataset registry (fill in)

### Dataset 1: Corrections Statistical Analysis Tool: Prisoners

- **Source:** https://csat.bjs.ojp.gov/advanced-query
- **License:** These data are provided by the Bureau of Justice Statistics, which is required to disseminate their data in a method that is accessible to the public and usable for statistical or research purposes.
- **Date pulled:** 2026-22-05
- **Approximate size:** 2,376 rows x 3 columns, 22 kb
- **Owner on this project:** Emery Kerani
- **Where it lives in this repo:** `data/raw/annual_prison_counts.xlsx` 
- **Ethics / consent notes:** Already de-identified and aggregated
- **How to fetch (for a teammate cloning fresh):** Select *Annual Counts* for query type, *Year-end Population* for category, *All* for sex, *Total Year-end Population* for variable 1, and *All* for juridiction and year.

### Dataset 2: Number of Poor and Poverty Rate by State

- **Source:** https://www.census.gov/data/tables/time-series/demo/income-poverty/historical-poverty-people.html
- **License:** These data are made available by the Census Bureau, under the condition that the Census Bureau is cited as the original data source.
- **Date pulled:** 2026-22-05
- **Approximate size:** 2,350 rows x 6 columns, 87 kb
- **Owner on this project:** Emery Kerani
- **Where it lives in this repo:** `data/raw/hstpov19.xlsx` 
- **Ethics / consent notes:** Data has already been de-identified and aggregated
- **How to fetch (for a teammate cloning fresh):** Go to the URL and download table 19. 

### Dataset 3: Summary Reporting System: Estimated Crimes

- **Source:** https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads
- **License:** These data are provided as part of the FBI's Crime Data Explorer page, which makes data on a variety of crimes publicly available. 
- **Date pulled:** 2026-22-05
- **Approximate size:** 2,389 rows x 15 columns, 207 kb
- **Owner on this project:** Emery Kerani
- **Where it lives in this repo:** `data/raw/estimated_crimes_1979_2024.csv`
- **Ethics / consent notes:** Data has already been de-identified and aggregated
- **How to fetch (for a teammate cloning fresh):** Access the website, scroll down to the Additional Datasets tab, select the Summary Reporting System dropdown, and hit the download button.

### Dataset 4: IPUMS CPS

- **Source:** https://cps.ipums.org/cps-action/variables/group
- **License:** These data are collected by the IPUMS Current Population Count Survey; the survey must be properly cited along with the CPS source data.
- **Date pulled:** 2026-06-06
- **Approximate size:** 12,821,891 rows x 17 columns, 1,521,110 kb
- **Owner on this project:** Emery Kerani
- **Where it lives in this repo:** NA (too large, lives in R)
- **Ethics / consent notes:** Data have been de-identified but are at the household level and will need to be aggregate. Terms of use require that the title and citation of the project is provided to IPUMS via their bibliography tool.
- **How to fetch (for a teammate cloning fresh):** Select samples, then select all years from 1980-2020 under the ASEC tab and select submit sample selections. In the select variables screen, go to household > core > geographic and add STATEFIP to cart. Under person > core > demographics add RACE to the cart. Then select view cart and create data extract. Download the .dat file provided, as well as the DDI as an .xml file, and move them to an appropriate folder. Then in R, download the `ipumsr` package and run:
`ddi <- read_ipums_ddi("./capstone/cps_00001.xml")`
`data <- read_ipums_micro(ddi)`

### Dataset 5: Police Spending

- **Source:** https://state-local-finance-data.taxpolicycenter.org/pages.cfm#
- **License:** These data are compiled by the Urban Institute based on data collected and released by the Census Bureau; both institutions should be recognized in a citation. 
- **Date pulled:** 2026-09-06
- **Approximate size:** In order: 2,030 rows x 6 columns, 613 kb
- **Owner on this project:** Emery Kerani
- **Where it lives in this repo:** `data/raw/police_spending_all.xls`
- **Ethics / consent notes:** Data do not concern individual people but rather government spending
- **How to fetch (for a teammate cloning fresh):** Access the Urban Institute's site via the url above; hit the get starte button; select *State and Local* as the level of government; select all states; select items E087, E088, and E089 for the series; select years 1980-2020; select *per capita* for the units and *real* under nominal/real; hit view results and export as an excel.
