# Fusion-Lakehouse-Dashboard for New York Yellow Taxi Trip Dataset


## Dataset

The yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts from year 2018. The data used in the attached datasets were collected and provided to the NYC Taxi and Limousine Commission (TLC) by technology providers authorized under the Taxicab & Livery Passenger Enhancement Programs (TPEP/LPEP). The data set, container 112M rows and 17 columns, is stored in a CSV file about 9.71GB in size.

Source:  https://data.cityofnewyork.us/Transportation/2018-Yellow-Taxi-Trip-Data/t29m-gskq


## Resources

1. Fusion = [IBM Storage Fusion](https://www.ibm.com/products/storage-fusion) SDS V2.5 installed with OpenShift in IBM Cloud VPC
2. Lakehouse = [watsonx.data](https://www.ibm.com/products/watsonx-data) v1.0
3. Dashboard = [Cognos Analytics Server](https://www.ibm.com/products/cognos-analytics) V11.2


## Workflow

1. Prepare dataset by downloading CSV file locally then uploading to an object storage
2. Create Lakehouse/Fusion Catalog, Schema and Table connecting to the dataset (CSV) in object storage
3. Filter and transform the original CSV file into a more efficient Lakehouse table (ORC)
4. Connect to the Lakehouse/Fusion from Dashboard to create visualization of dataset
