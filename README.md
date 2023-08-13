# S4WX Demo: Fusion/Lakehouse for Dashboarding NY Yellow Taxi Data Set


## Dataset

The yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts from year 2018. The data used in the attached datasets were collected and provided to the NYC Taxi and Limousine Commission (TLC) by technology providers authorized under the Taxicab & Livery Passenger Enhancement Programs (TPEP/LPEP).

Source:  https://data.cityofnewyork.us/Transportation/2018-Yellow-Taxi-Trip-Data/t29m-gskq


## Technologies

1. Fusion = IBM Storage Fusion 2.5 installed with OpenShift in IBM Cloud VPC
2. Lakehouse = IBM watsonx.data v1.0
3. Dashboard = IBM Cognos Analytics Server 11.2


## Workflow

1. Prepare dataset by downloading locally first then reloading to an object storage
2. Create Lakehouse/Fusion (WXD100@Fusion101) Catalog, Schema and Table connecting to the dataset (CSV) in object storage
3. Filter and transform the original CSV file into a more efficient Lakehouse table (ORC)
4. Connect to the Lakehouse/Fusion (WXD100@Fusion101) 
