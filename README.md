# SparkStreamingExercise

Start All Servers
**********************************************************************************


#Start Zookeeper Server
  cd /usr/local/kafka
  zookeeper-server-start etc/kafka/zookeeper.properties 

#Start Kafka Server
  cd /usr/local/kafka
  kafka-server-start etc/kafka/server.properties

#Create topic
  kafka-topics --zookeeper localhost:2181 --create --topic creditcardTransaction  --replication-factor 1 --partitions 3 

 #Spark Cluster Setup  
    #Start Spark Master
      start-master.sh
  
    #Start Spark Slave
      start-slave.sh spark://kehaque634:7077  

    #Access Spark Web UI
      http://vm_ip:8080/ 

#Start Cassandra Server
cassandra -f

#Connect to Cassandra Server through Cassandra console client
cqlsh
 

