# pythonChat
python chat app connected with java app with kafka as a middleware.
#kafka steps
1 bin/zookeeper-server-start.sh config/zookeeper.properties 

2  bin/kafka-server-start.sh config/server.properties 

3 bin/kafka-topics.sh --create --topic chat --bootstrap-server localhost:9092 
--replication-factor 1 --partitions 1 
4 bin/kafka-console-producer.sh --topic chat --bootstrap-server localhost:9092

5 bin/kafka-console-consumer.sh --topic chat --from-beginning --bootstrap-server localhost:9092

#python package
pip install kafka-python
