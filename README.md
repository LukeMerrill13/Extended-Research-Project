# Extended_Research_Project

This repository contains all of the Python code required to reproduce the results presented in the Extended Research Project (ERP). 

## Data 

Three publicly available datasets were used in the making of the report:
1)	Energy generation data by fuel type
* This dataset was downloaded from: https://bmrs.elexon.co.uk/generation-by-fuel-type and is imported into ‘Marginal_Emission_Factors.ipynb’
* Data was downloaded for observations between: 00:00 on 01/08/2022 and 23:30 on 31/07/2025

4)	Smart meter data
•	This dataset was downloaded from: https://data.london.gov.uk/dataset/smartmeter-energy-use-data-in-london-households/ and is imported into ‘Smart_Meter_Data.ipynb’
•	The data selected from this page is the partitioned zip file containing 168 separate CSV files

5)	Market index prices
•	This dataset was downloaded from: https://bmrs.elexon.co.uk/market-index-prices and is imported into ‘Market_Index_Prices.ipynb’
•	Data was downloaded for observations between: 00:00 on 24/08/2025 and 23:30 on 31/07/2025


## Python Scripts

Five python scripts are used to produce the results presented in the extended report. The following scripts can be run independently of each other: 

•	Marginal_Emission_Factors.ipynb imports the energy generation data and produce estimates of marginal factors.
•	Smart_Meter_Data.ipynb downloads and pre-processes the smart meter data
•	Market_Index_Prices.ipynb downloads and pre-process the market pricing data.
•	Demand_Modelling.ipynb models elasticity matrices for different consumer groups

The final script, Price_Optimisation.ipynb, imports the outputs from the aforementioned notebooks and runs the pricing optimisation models which produce the main findings from this report.




