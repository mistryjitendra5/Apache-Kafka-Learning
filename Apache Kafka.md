# Apache Kafka

Kafka is a distributed Message streaming platform that uses publish and subscribe mechanism to stream the records.

Originally developed by LinkedIn and later donated to Apache foundation. Kafka is a open source.

| ![image](https://user-images.githubusercontent.com/79099288/177265955-d6c2b941-0c22-4180-9de2-e2319819f5d4.png)

# Messaging Systems
A messaging system is responsible for transferring data from one application to another so the applications can focus on without getting bogged down on data transmission and sharing.

# Point to Point Messaging Systems
1. Messages are persisted in a Queue.
2. A particular message can be consumed by a maximumof one receiver only.
3. There is no time dependency laid for the receiver to receive the message.
4. When the Receiver receives the message, it will send an acknowledgement back to the Sender.

# Publish-Subscribe Messaging Systems
1. Messages are persisted in a Topic.
2. A particular message can be consumed by any number of consumers.
3. There is no time dependency laid for the consumer to consumer the message.
4. When the Subscriber receives the message, it does not send an acknowledgement back to the Publisher.

# Message Streams
1. A stream of messages belonging to a particular category is called a topic.
2. It is a logical feed name to which records are published.
3. Similar to a table in a database.
4. Unique identifier of a topic is its NAME.
5. We can create as many topics as we want.

# Topics
1. Topics are splitted in Partitions.
2. All the messages withing a partition are ordered and immutable.
3. Each message within a partition has a unique id associated knowns as Offset.

# Replicas
1. Replicas are backup of a partition
2. Replicas are never read or write data.
3. They are used to prevent data lost. (Fault-Tolerance)

# Producer
1. Producers are applications which write/publish data to the topics within a cluster using the Producting APIs.
2. Producers can write data either on the topic level (All the partitions of that topic) or specific partitions of the topic.

# Consumer
1. Consumers are applications which read/consume data from the topics within a cluster using the Consuming APIs.
2. Consumers can read data either on the topic level (All the partitions of that topic) or specific partitions of the topic.
3. Consumers are always associated with exactly one Cunsumer Group.
4. A Consumer Group is a group of related consumers that perform a task.

# Broker
1. Broker are simple software processes who maintain and manage the published messages and also known as Kafka servers.
2. Brokers also manage the consumer-offsets and are responsible for the delivery of messages to the right consumers.
3. A set of brokers who are communicating with each other to perform the management and maintenance task are collectively known as Kafka Cluster.
4. We can add more brokers in a already running Kafka Cluster without any downtime.

# Zookeeper
1. Zookeeper is used to monitor Kafka Cluster and co-ordinate with each broker. It keeps all the metadata information related to kafka cluster in the forms of key-value pair. Metadata includes:
a. Configuration information
b. Health status of each broker
2. It is used for controller election within Kafka Cluster.
3. A set of Zookeeper nodes wotrking together to manage other distributed systems is knowns as Zookeeeper Cluster or Zookeeper Ensemble.
