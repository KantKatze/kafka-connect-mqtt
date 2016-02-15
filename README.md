# Mqtt to Apache Kafka Connect [![Build Status](https://travis-ci.org/evokly/kafka-connect-mqtt.svg?branch=master)](https://travis-ci.org/evokly/kafka-connect-mqtt)

## Prerequisites
* [Apache Kafka](https://kafka.apache.org/) (0.9.x version) is publish-subscribe messaging rethought as a distributed commit log. 

## Usage
**For development:**

* run check (checkstyle, findbugs, test):  
  `./gradlew clean check`

* run project:  
  `connect-standalone.sh /usr/local/etc/kafka/connect-standalone.properties config/mqtt.properties`
    * libs needs to be added to CLASSPATH:
        * `kafka-connect-mqtt-{project.version}.jar`
        * `org.eclipse.paho.client.mqttv3-1.0.2.jar`

**For production:**

* build project: `./gradlew clean jar` - output `./build/libs`

* generate API documentation: `./gradlew javadoc` - output `./build/docs/javadoc`

## License
See [LICENSE](LICENSE) file for License