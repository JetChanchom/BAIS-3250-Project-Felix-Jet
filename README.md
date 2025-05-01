# BAIS-3250-Project-Felix-Jet
Felix Menges, Jet Chanchom

Files in the Scripts folder:
- Data Files
    - January 2025 Complete Monthly Ridership (with adjustments and estimates)_250303.xlsx
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