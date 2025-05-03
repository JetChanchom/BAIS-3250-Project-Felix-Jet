# BAIS-3250-Project-Felix-Jet

![Python badge](https://img.shields.io/static/v1?message=python&logo=python&labelColor=5c5c5c&color=3776AB&logoColor=white&label=%20&style=for-the-badge)

Contributors: Felix Menges, Jet Chanchom

Final project for BAIS:3250 Data Wrangling analyzing rail-based forms of public transportation in the United States.

## Table of Contents

Files in the Scripts folder:

- Data Files
  - January 2025 Complete Monthly Ridership (with adjustments and estimates)\_250303.xlsx
    - [Source](https://www.transit.dot.gov/ntd/data-product/monthly-module-adjusted-data-release)
  - alltransit100k.csv
    - Created by webscrape-FelixJet.ipynb
  - alltransit-railridership_cleaned.csv
    - Compiled, cleaned, & integrated data from dataIntegration-FelixJet.ipynb
- Python Scripts
  - analysis-FelixJet.ipynb
    - Data analysis derived from charts, contains regression, plots, and summaries
  - dataIntegration-FelixJet.ipynb
    - Compiles the January.xlsx & alltransit100k.csv into alltransit-railridership_cleaned.csv
  - webscrape-FelixJet.ipynb
    - Scraped [source](https://alltransit.cnt.org/rankings/)

## Data Dictionary

| Field | Data | Description |
| --- | --- | --- |
| Agency | Text | Name of service provider agency
| Mode | Text | Mode of transportation: <ul><li>Alaska Railroad (AR)</li><li>Cable car (CC)</li><li>Commuter rail (CR)</li><li>Heavy rail (HR)</li><li>Hybrid rail (YR)</li><li>Inclined plane (IP)</li><li>Light rail (LR)</li><li>Monorail/Automated guideway transit (MG)</li><li>Streetcar (SR)</li></ul> |
| Type of Service (TOS) | Text | How services are provided: <ul><li>Directly operated (DO)</li><li>Purchased transportation (PT)</li></ul> |
| Headquarters (HQ) City| Text | City of Agency’s Headquarters |
| HQ State Text | State of Agency’s Headquarters |
| Urbanized Area (UZA) SQ Miles | Numeric | The size of the Urbanized Area (UZA), a region containg at least 50,000 people |
| UZA Population | Numeric | The population of the UZA|
| Service Area Population Numeric | The population within a service area (a ¾ mile radius surrounding a rail station)
| Service Area SQ Miles | Numeric | Total area covered by the service area |
| Unlinked Passenger Trips (UPT) | Numeric | Total number of times a person has boarded the railway |
| Avg Trip Length | Numeric | Average length of trip |
| Fares | Numeric | Total revenue made from fares |
| Operating Expenses Numeric | otal expenses from operating the railway|
| Avg Cost per Trip | Numeric | Expenses divided by total number of trips |
| Avg Fares per Trip | Numeric | Total fares divided by total number of trips |
| Year | Numeric | Year of data collected |
| Vehicle Revenue Miles (VRM)| Numeric | Actual & scheduled miles during revenue service (excluding maintenance & training) |
| Rank | Numeric | Ranking amongst other regions |
| Name | Text | Name of City & State|
| Score | Numeric | Overall Transit Score weighted by TCI, # of Jobs, and average Trips per Week. Higher score means better transit service. Scaled [0.0:10.0] |
| Transit Connectivity Index (TCI) | Numeric | A normalized ranking of the sum of weekly bus & train traffic per region. Higher ranking means denser transit connectivity. Scaled [0:100] |
| Jobs | Numeric | Jobs within 30-minute access of public transport |
| Trips/Week | Numeric | Transit Trips per Week within ½ Mile |
| Routes | Numeric | Total number of Transit Routes within ½ Mile |
| Transit Shed | Numeric | Size of geographic area accessible within 30 minutes by public transportation in square miles |
| %Transit | Numeric | % of commuters who use transit |
| Population | Numeric | Population of Region |
