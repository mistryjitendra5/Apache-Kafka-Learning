# APACHE KAFKA:

Kafka is a distributed Message streaming platform that uses publish and subscribe mechanism to stream the records.

Originally developed by LinkedIn and later donated to Apache foundation. Kafka is a open source.

| ![image](https://user-images.githubusercontent.com/79099288/177265955-d6c2b941-0c22-4180-9de2-e2319819f5d4.png)

# MESSAGING SYSTEMS:
A messaging system is responsible for transferring data from one application to another so the applications can focus on without getting bogged down on data transmission and sharing.

# Point to Point Messaging Systems
1. Messages are persisted in a Queue.
2. A particular message can be consumed by a maximumof one receiver only.
3. There is no time dependency laid for the receiver to receive the message.
4. When the Receiver receives the message, it will send an acknowledgement back to the Sender.

# Publish-Subscribe Messaging System
1. Messages are persisted in a Topic.
2. A particular message can be consumed by any number of consumers.
3. There is no time dependency laid for the consumer to consumer the message.
4. When the Subscriber receives the message, it does not send an acknowledgement back to the Publisher.
