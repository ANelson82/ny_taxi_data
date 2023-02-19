# New York Taxi Data

# Steps
1. Investigate the Data from the BigQuery Public Datasets. [NYC Taxi Dataset](https://console.cloud.google.com/marketplace/details/city-of-new-york/nyc-tlc-trips)
1. Export the data to the Google Cloud Storage Buck
```
  EXPORT DATA OPTIONS(
  uri='gs://bucket/folder/*',
  format='PARQUET') AS
  SELECT * FROM mydataset.table1 ORDER BY field1 LIMIT 10
  ```
1. Combine the parquet files into a single file using Python and DuckDB
1. Import the Parquet tnto PowerBI
1. Download the Taxi Zone Lookup Table and Taxi Zone Shapefile from [NYC](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
1. Convert to Topo JSON format uksing [mapshaper](https://mapshaper.org/)
1. 
