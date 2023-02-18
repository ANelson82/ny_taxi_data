# New York Taxi Data

# Steps
1. Investigate the Data from the BigQuery Public Datasets. [NYC Taxi Dataset](https://console.cloud.google.com/marketplace/details/city-of-new-york/nyc-tlc-trips)
1. Export the data to the Google Cloud Storage Buck
```EXPORT DATA OPTIONS(
  uri='gs://bucket/folder/*',
  format='PARQUET') AS
  SELECT * FROM mydataset.table1 ORDER BY field1 LIMIT 10
  ```
1. Combine the parquet files into a single file using Python and DuckDB
1. Import Into PowerBI
1. 
