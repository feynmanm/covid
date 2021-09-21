# Comparing Covid 19 trends across US Counties
This repository attempts to predict US county Covid 19 case densities (cases per unit of population) and vaccination rates in the CAN (Covid Act Now) notebooks (.ipynb files). Classic machine-learning models here, no deep learning, as the examples are applied to individual US counties (of which there are around 3000).

## CAN notebooks
These two notebooks -- which explore Covid Act Now data -- are the most useful are far as predicting something

To run the CAN notebooks, you would need to download the counties.timeseries.csv file (245MB) from https://apidocs.covidactnow.org/#register and store it in your working covid data directory as such:  
- ..\covid\data\CANdata\counties.timeseries.csv

You would also need to first run the exploration notebook to create the correct pickle file for the predictions notebook to read.

## CDC notebooks
This set of notebooks extracts county-by-county CDC data on positive Covid 19 testing, hospitalizations, and populations. I haven't successfully found something meaningful to predict yet, but much interesting exploratory work abounds, and there is plenty more to explore (effort is ongoing).  

To run the CDC notebooks as is, you would need to download the CDC cases with geography file (3.8GB) from https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-with-Ge/ynhu-f2s2 and store it in the covid data directory as such:  
- ..\covid\data\CDCdata\COVID-19_Case_Surveillance_Public_Use_Data_with_Geography.csv

You would need to download the CDC hospital patient file (106MB) from https://healthdata.gov/Hospital/COVID-19-Reported-Patient-Impact-and-Hospital-Capa/anag-cw7u and store it in the covid data directory as such:  
- ..\covid\data\CDCdata\COVID-19_Reported_Patient_Impact_and_Hospital_Capacity_by_Facility.csv

You would also need to run the following notebooks: hosp_raw, cases  
and then run: counties, patients  
and then you can run: Hospitalization_Rate

Note, the following notebooks are also in the repo, but are largely superceded: cases_investigation, covid19_sorna, covid19_nublar
