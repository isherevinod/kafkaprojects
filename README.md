# kafkaprojects
Kafka related project demo



*****************************Kafka commanda****************************************************
correct kafka working main version  kafka_2.12-3.2.0 and placed at below location
C:\kafka

set path=%path%;C:\Users\vinodkumar.chidar\Downloads\Java\jdk1.8.0_202\bin
--------------------------------------
C:\kafka\bin\windows>zookeeper-server-start.bat C:\kafka\config\zookeeper.properties
---------------------------
C:\kafka\bin\windows>kafka-server-start.bat C:\kafka\config\server.properties
---------------------------------------------
C:\kafka\bin\windows>kafka-topics.bat --create --topic javatechie --bootstrap-server localhost:9092  ----this is correct for new Newer versions(2.2+) of Kafka no longer requires ZooKeeper connection string

C:\kafka\bin\windows>kafka-topics.bat --create --topic javatechie-stream --bootstrap-server localhost:9092

---List for topics need to check
C:\kafka\bin\windows>kafka-topics.bat --list --bootstrap-server localhost:9092
----------------------------------------
C:\kafka\bin\windows>kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic javatechie
