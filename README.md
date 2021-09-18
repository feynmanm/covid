# Comparing Covid 19 trends across US Counties
Machine learning notebooks (.ipynb files) predicting case density (cases per unit of population) and vaccination rate in the CAN notebooks. Classic machine-learning models here, no deep learning, as the examples are applied to individual US counties (of which there are around 3000).

## CAN notebooks
These two notebooks are the most useful are far as predicting something

To run the notebooks based on the Covid Act Now data (CANnotebooks), you would need to download the counties.timeseries.csv file (245MB) from https://apidocs.covidactnow.org/#register and store it in your working covid data directory as such:  
- ..\covid\data\CANdata\counties.timeseries.csv

You would also need to first run the exploration notebook to create the correct pickle file for the predictions notebook to read in

## CDC notebooks
This set of notebooks attempts to discover something that can be modeled from CDC data. It is not directly successful in this regard, but there is a lot of interesting exploratory work.

To run the CDC notebooks, you would need to download the CDC cases with geography file (3.8GB) from https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-with-Ge/ynhu-f2s2 and store it in the covid data directory as such:  
- ..\covid\data\CDCdata\COVID-19_Case_Surveillance_Public_Use_Data_with_Geography.csv

You would need to download the CDC hospital patient file (106MB) from https://healthdata.gov/Hospital/COVID-19-Reported-Patient-Impact-and-Hospital-Capa/anag-cw7u and store it in the covid data directory as such:  
- ..\covid\data\CDCdata\COVID-19_Reported_Patient_Impact_and_Hospital_Capacity_by_Facility.csv

You would also need to run the following notebooks: hosp_raw, cases  
and then run: counties, patients  
and then you can run: Hospitalization_Rate

And these notebooks are independent of others: cases_investigation, covid19_sorna, covid19_nublar
