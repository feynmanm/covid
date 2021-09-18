# covid
Machine learning notebooks (.ipynb files) predicting case density (cases per unit of population) and vaccination rate

In addition to the files stored in the repo...  

To run the notebooks based on the Covid Act Now data (CANnotebooks), you would need to download the counties.timeseries.csv file (245MB) from https://apidocs.covidactnow.org/#register and store it in your working covid data directory as such:  
- ..\covid/data/CANdata/counties.timeseries.csv

To run the CDC notebooks, you would need to download the CDC cases with geography file (3.8GB) from https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-with-Ge/ynhu-f2s2 and store it in the covid data directory as such:  
- ..\covid\data\CDCdata\COVID-19_Case_Surveillance_Public_Use_Data_with_Geography.csv

You would need to download the CDC hospital patient file (106MB) from https://healthdata.gov/Hospital/COVID-19-Reported-Patient-Impact-and-Hospital-Capa/anag-cw7u and store it in the covid data directory as such:
- ..\covid\data\CDCdata\COVID-19_Reported_Patient_Impact_and_Hospital_Capacity_by_Facility.csv
