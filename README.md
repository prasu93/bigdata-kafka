# bigdata-kafka

## Download
- Download Kafka [here](https://www.apache.org/dyn/closer.cgi?path=/kafka/2.6.0/kafka_2.13-2.6.0.tgz)

## Steps for starting Kafka service

- zookeeper service: Run Powershell as an Administrator in the kafka source folder and run the command: .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
- kafka service: Run Powershell as an Administrator in the kafka source folder and run the command: .\bin\windows\kafka-server-start.bat .\config\server.properties
- My topics: "northwest-subjects", "car-models"
- Start the kafka producer: .\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic northwest-subjects
- After that, we can enter messages related.
- Start the kafka consumer: .\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic northwest-subjects --from-beginning
- Here we can receive the messages.
