# sparkStreamingGraphAnalitics

Before starting executing these code, you have should have already:

* Kafka server running
* Kafka Topic shoud be created.
* kafka producer and consumer console started for testing purpose.


### Some Useful Kafka Commands
Start Zookeeper
zookeeper-server-start.sh config\zookeeper.properties

Start Kafka Broker
kafka-server-start.sh config/server.properties

Create topic
kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test

List topic
kafka-topics.sh --list --zookeeper localhost:2181

Start Producer
kafka-console-producer.sh --broker-list localhost:9092 --topic test

Receive message
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
