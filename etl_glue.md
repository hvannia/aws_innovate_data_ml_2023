# ETL with GLUE

## Data Integration Engines
* AWS Glue for Apache Spark
* AWS Glue for Ray (preview)
use oython libs
* AWS Glue for Python Shell (python 3.10)
s-m sized jobs
* AWS Flexible Execution 
non-urgent worloads, uses spare capacity, non-urgent SLA

## Connectors
Native support for Hudi, Delta Lake & Iceberg
Third party( slack, salesforce, slack, goodle analytics) SaaS sourced data -> Amazon AppFlow-> S3 -> Glue Catalog

Souces:
Built-In
Marketaplace
Custom

## Interfaces
Glue studio - SQL , python, Apache Spark, Scala
Data Brew - Clean and normalize data using a visual interface, profile data 
Interactive Sessions API - Use favorite IDE or SageMaker 

## Operationalize 
Orchestrate workflows:
- AWS Glue Workflows
- Amazon Managed workflow for Apache Airflow 
- AWS Step functions

## Version control
Github
AWS Glue JObs
AWS CodeCommit

## Monitoring
RCA, debugging recommendations and logs 

## Data Management 
Glue Catalog - > apache Hive compatible 
Schema Registry - Kafka integration 

## Senstive data Detection 
Senstivie data Detection across TB of data - remediate ( store, redact, mask, replace)

## Data Quality
Glue Data Catalog - recommend data quaity rules (preview)
Can create an evaludate data quality in the data pipeline 

