# Extended_Research_Project

This repository contains all of the Python code required to reproduce the results presented in the Extended Research Project (ERP). The details below explain how to source the exact datasets used and the order in which each script should be executed.

## Data 

Three publicly available datasets were used in the making of the report:
1)	Energy generation data by fuel type
* This dataset was downloaded from: https://bmrs.elexon.co.uk/generation-by-fuel-type and is imported into ‘Marginal_Emission_Factors.ipynb’
* Data was downloaded for observations between: 00:00 on 01/08/2022 and 23:30 on 31/07/2025

2)	Smart meter data
* This dataset was downloaded from: https://data.london.gov.uk/dataset/smartmeter-energy-use-data-in-london-households/ and is imported into ‘Smart_Meter_Data.ipynb’
* The data selected from this page is the partitioned zip file containing 168 separate CSV files

3)	Market index prices
* This dataset was downloaded from: https://bmrs.elexon.co.uk/market-index-prices and is imported into ‘Market_Index_Prices.ipynb’
* Data was downloaded for observations between: 00:00 on 24/07/2025 and 23:30 on 31/07/2025


## Python Scripts

Five python scripts are used to produce the results presented in the report. To run these sripts, open the notebooks within this repository in Jupyter. Import the datasets as described and run all cells in order. The following scripts can be run independently of each other: 

* Marginal_Emission_Factors.ipynb imports the energy generation data and produce estimates of marginal factors.
* Smart_Meter_Data.ipynb downloads and pre-processes the smart meter data
* Market_Index_Prices.ipynb downloads and pre-process the market pricing data.
* Demand_Modelling.ipynb models elasticity matrices for different consumer groups

The final script, Price_Optimisation.ipynb, relies on the outputs from the aforementioned scripts. It uses them to run the pricing optimisation models which produce the report's main findings.




