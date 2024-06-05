Steps:

<ol>
  <li>Download and extract Kafka

    wget https://archive.apache.org/dist/kafka/3.5.1/kafka_2.12-3.5.1.tgz

    tar -xzf kafka_2.12-3.5.1.tgz   
  </li>
  <li>Start ZooKeeper

    cd kafka_2.12-3.5.1

    bin/zookeeper-server-start.sh config/zookeeper.properties
    
  </li>
  <li>Start the Kafka broker service

    cd kafka_2.12-3.5.1

    bin/kafka-server-start.sh config/server.properties

    
  </li>
  <li>Create a topic in the Admin.py file

    cd kafka_2.12-3.5.1
    
    Install the kafka-python package by running the following command: pip3 install kafka-python
        
    Create a new file named admin.py and write the python code to create a topic
    
  </li>
  <li>Create Producer.py file

    Create a new file named producer.py and write the python code to publish the data to a topic
  </li>
  <li>Create Consumer.py file

    Create a new file named consumer.py and write the python code to consume data from a topic
  </li>
  <li>Execute the three Python files
    
    python3 admin.py
    python3 producer.py
    python3 consumer.py
  </li>
 
</ol>
