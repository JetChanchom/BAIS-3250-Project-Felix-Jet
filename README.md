# BAIS-3250-Project-Felix-Jet

![Python badge](https://img.shields.io/static/v1?message=python&logo=python&labelColor=5c5c5c&color=3776AB&logoColor=white&label=%20&style=for-the-badge) ![Selenium](https://img.shields.io/badge/-selenium-%43B02A?style=for-the-badge&logo=selenium&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

Contributors: Felix Menges, Jet Chanchom

Final project for BAIS:3250 Data Wrangling analyzing rail-based forms of public transportation in the United States.

## Table of Contents

Files in the Scripts folder:

- Data Files
  - January 2025 Complete Monthly Ridership (with adjustments and estimates)\_250303.xlsx
    - [Source](https://www.transit.dot.gov/ntd/data-product/monthly-module-adjusted-data-release)
  - alltransit10k.csv
    - Created by webscrape-FelixJet.ipynb
  - alltransit-railridership_cleaned.csv
    - Compiled, cleaned, & integrated data from dataIntegration-FelixJet.ipynb
- Python Scripts
  - analysis-FelixJet.ipynb
    - Data analysis derived from charts, contains regression, plots, and summaries
  - dataIntegration-FelixJet.ipynb
    - Compiles the January.xlsx & alltransit10k.csv into alltransit-railridership_cleaned.csv
  - webscrape-FelixJet.ipynb
    - Scraped [source](https://alltransit.cnt.org/rankings/)

## Data Dictionary

| Field                            | Data    | Description                                                                                                                                                                                                                                                                                   |
| -------------------------------- | ------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Agency                           | Text    | Name of service provider agency                                                                                                                                                                                                                                                               |
| Mode                             | Text    | Mode of transportation: <ul><li>Alaska Railroad (AR)</li><li>Cable car (CC)</li><li>Commuter rail (CR)</li><li>Heavy rail (HR)</li><li>Hybrid rail (YR)</li><li>Inclined plane (IP)</li><li>Light rail (LR)</li><li>Monorail/Automated guideway transit (MG)</li><li>Streetcar (SR)</li></ul> |
| Headquarters (HQ) City           | Text    | City of Agency’s Headquarters                                                                                                                                                                                                                                                                 |
| HQ State                         | Text    | State of Agency’s Headquarters                                                                                                                                                                                                                                                                |
| Service Area SQ Miles            | Numeric | Total area covered by the service area                                                                                                                                                                                                                                                        |
| Unlinked Passenger Trips (UPT)   | Numeric | Total number of times a person has boarded the railway                                                                                                                                                                                                                                        |
| Avg Cost per Trip                | Numeric | Expenses divided by total number of trips                                                                                                                                                                                                                                                     |
| Avg Fares per Trip               | Numeric | Total fares divided by total number of trips                                                                                                                                                                                                                                                  |
| Year                             | Numeric | Year of data collected                                                                                                                                                                                                                                                                        |
| Vehicle Revenue Miles (VRM)      | Numeric | Actual & scheduled miles during revenue service (excluding maintenance & training)                                                                                                                                                                                                            |
| Name                             | Text    | Name of City & State                                                                                                                                                                                                                                                                          |
| Transit Connectivity Index (TCI) | Numeric | A normalized ranking of the sum of weekly bus & train traffic per region. Higher ranking means denser transit connectivity. Scaled [0:100]                                                                                                                                                    |
| Jobs                             | Numeric | Jobs within 30-minute access of public transport                                                                                                                                                                                                                                              |
| Trips/Week                       | Numeric | Transit Trips per Week within ½ Mile                                                                                                                                                                                                                                                          |
| Routes                           | Numeric | Total number of Transit Routes within ½ Mile                                                                                                                                                                                                                                                  |
| %Transit                         | Numeric | % of commuters who use transit                                                                                                                                                                                                                                                                |
| Population                       | Numeric | Population of Region                                                                                                                                                                                                                                                                          |
