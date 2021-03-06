# Apache Kafka (Experimental)

### Info:

 This template creates, scale in and scale out a multinodes kafka broker cluster on top of k8s. The configuration is generated with confd from k8s. 
 Cluster size are variable after deployment, and get reconfigured.
 
 
### Usage:

 Select Apache Kafka from catalog. 
 
 Enter the number of nodes, mem and refresh interval for the kafka cluster.
 
 Change the following kafka default parameters, if you need:

- KAFKA_LOG_DIRS="/opt/kafka/logs"
- KAFKA_LOG_RETENTION_HOURS="168"
- KAFKA_NUM_PARTITIONS="1"
- KAFKA_DELETE_TOPICS="false"
- ADVERTISE_PUB_IP= < true | false >

 Select zookeeper stack/service to connect to.
 
 Click deploy.
 
 Kafka can now be accessed over the Rancher network. 

 Note: When you scale the cluster, zero downtime is not guaranteed..yet..
