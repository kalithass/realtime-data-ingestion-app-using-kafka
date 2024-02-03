# Getting started
* Download kafka and run following commands inside  kafka-version/bin/windows to run kafka.

      zookeeper-server-start.bat ../../config/zookeeper.properties

      kafka-server-start.bat ../../config/server.properties

* First run the producer app to read data from wikimedia. Use the following command to check whether the data has been sent to kafka topic.
 

      kafka-console-consumer.bat --topic topic_name --from-beginning --bootstrap-server localhost:9092

* Run the consumer app. Now the realtime data will be getting stored into database.
