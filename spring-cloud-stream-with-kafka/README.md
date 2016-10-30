## Spring Cloud Stream POC

### Goal

This POC demonstrates spring integration with `Kafka`.

* A random message is sent every seconds by a producer to an `input` topic.
* A consumer transforms messages coming from the `input` topic and sends the result to an `output` topic.
* A consumer finally prints messages received from the `output` topic.

Each step is supposed to be run in a dedicated `JVM`, that's why communication must be done through `Kafka`.

### Use the sample

You need to run `Kafka` and `Zookeeper` locally.