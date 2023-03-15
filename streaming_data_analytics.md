Build_modern_data_streaming_analytics__architectures_on_AWS.pdf



## Kinesis Data Streams
## KDA for Apache
## Kinesis Data Firehose

## Managed Streaming for Kafka (MSK)


## Patterns
### Clickstream 
Use cases:
campaign optimization
generate baluable insights
tracking for customers online jurney
realtime upselling and cross seling 


Data Ingestion -> Kinesis Streams or MSK
[Real time analytics]
    KInesis Data Analytics -> Cloudwatch
[batch analytics]
    Kinesis Data Firehose -> S3 -> Quicksight 



### Log Analytics
Use cases:
realtime application and infrastructrure monitoring
Root-cause analysis
Security intelligence and event management (SIEM)

Data collection ->
    App Logs
    VPC Flow los
    Cloudytrail logs
    Cloudwatch logs
Kinesis Data Streams ->
[realtime anomaly detection]
    KInesis data Analytics -> SNS
[near realtime analysis]
    Kinesis Data Firehose -> OpenSearch -> Opensearch dashboards


### Real time recommendations 
Use cases:
Tailored consumer exerience
personalized recommednations
user interaction based recommendations
instant feedback loop

API GW-> Kinesis Data Streams   -> Data Firehose -> S3 (persist)
                                -> lambda (consume) -> amazon personalize 

    lambda( get recommendations) -> API GW


### IoT
Use cases:
asset condition monitoring and predictive maintenance 
Suupply chain analytics
preactive quality assurance
fleet management 

Source ( IoTdevice) 0> AWS IoT GreenGrass ->() edge cloud ) 
    aws ingest 
        Iot Core .... 


### Change data Capture
USe cases:
Database replication and migration
Realtime infrmation distribution 
Audit log capture 


`ChangeDataCapture` pipeline with Amazon `MSK`
Aurora-> MSK Connect Debezium Mysql Connector -> (Kafka producer_ -> Amazon MSK Cluster (kafcka consumer) -> CDC Consume application 