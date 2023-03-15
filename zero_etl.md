# Zero ETL: Connect to all your data 

Connect to all your data across ingestion, analytics, machine learning, and business intelligence, as well as third-party data. With direct integrations between AWS services, we are eliminating ETL for common use cases.


## Federated query 
in amazon redshift and amazon athena
query between DS store R in S3
* Athena Datasource connectors 

SDK Query gneration - query in place 


## Machine learning preditions from data sources 
( without having to move data )

Aurora ML 
Neptune ML ( Deep Learning to graph data, no ml model)
Amazon Redshift ML (calls sagemaker autopilot to create a ML model )
Athena ML ( generate preditcions from a sagemaker ML model)


## Amazon Aurora Zero-ETL integration with Redshift
choose Aurora tables to analize in redshift
data flow is one directional, for transactional data to flow from Aurora to Redshift.


If you want to move data from Redshift to Aurora for some reason, can unload using UNLOAD command to S3 and then load to Aurora or use another technique.


## Data Exchange for Amazon Redshift 
find and subscribe to third party data 

## Data Exchange for S3 
Acces the same copu of the s3 obj that the data provider maintains 
(preview)

## Redshift auto copy from S3
Move large amounts of data  as soon as new files are created in S3 
Automate data loading without engineering resources 
(preview)  US East (N. Virginia), US East (Ohio), US West (Oregon), Asia Pacific (Tokyo), Europe (Ireland) and Europe (Stockholm). 

## AWS Glue 
serverless ETL and data integration service
built on Spak python and (eray?)


aws connects to... see slide deck-1 
tableau, servicenow, splunk, datadog, 

## Services for connection to 100s of data sources
Apppflow, Kinesis Data Firehouse, Athena, SageMaker, QuickSigt, DataSync, DataExchange, Glue

Redshift Streaming Ingestion  - Ingest data in data wharehouse
Kinesis or Kafka -> Kinesis Data Streams 