[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/Gau5_GFM)
## Requirements for Assignment #2
[Read the instruction](https://github.com/STIW3054-A232/class-activity-stiw3054/blob/main/Assignment-2.md)

## Assessment Criteria
[Check the rubrics](https://github.com/STIW3054-A232/class-activity-stiw3054/blob/main/Rubrics-Assignment-2.md)

## Your Info:
1. Matric Number & Name & Photo & Phone Number
2. Other related info (if any)

|    |                          NAME                            |           MATRIC NUMBER          |              PHONE NUMBER | PICTURE           |
| -- | -------------------------------------------------------- | -------------------------------- | --------------------------------------------- | ------- |
| 1. | <div align="center">MUHAMMAD DANIAL BIN MOHD FARIS</div> | <div align="center">294692</div> | <div align="center">(+60) 12 - 451 6452</div> | <div align="center"><img src="INSERT IMAGE URL HERE" alt="MUHAMMAD DANIAL BIN MOHD FARIS (294692)" width="100px"></div> |
| 2. | <div align="center">SHARWIN A/L PARAMESWARAN</div>       | <div align="center">295026</div> | <div align="center">(+60) 12 - 647 1786</div> | <div align="center"><img src="https://github.com/user-attachments/assets/8ef08b3b-4ea3-4b53-88fb-fcddd9eb182a" alt="SHARWIN A/L PARAMESWARAN (295026)" width="100px"></div> |

## Title: Real-Time Messaging with Apache Kafka in KRaft Mode
## Abstract (in 300 words)
   1. Background

      Apache Kafka is a powerful distributed messaging platform used for building real-time data pipelines. Traditionally, Kafka relied on Apache ZooKeeper for managing clusters, but with the introduction of KRaft mode, Kafka now handles cluster management itself, improving scalability and simplifying architecture. This assignment focuses on setting up Kafka in KRaft mode to create a producer-consumer application, where a Java-based producer sends data from a quotes API to a consumer over a network. By working with the latest version of Kafka (3.9.0) and KRaft mode, the project provides practical experience in real-time messaging and distributed system architecture.
      
   2. Problem Statement (from article)

      In the current digital era, efficient real-time data processing across distributed systems is crucial. Traditional messaging systems often struggle with scalability and performance. Apache Kafka offers a solution with high throughput and low latency, but it requires proper configuration. According to research by Kreps et al. (2011), Kafka is designed to provide high throughput, low latency, and fault tolerance, making it ideal for various real-time data integration tasks source. This assignment aims to provide practical experience with Apache Kafka in KRaft mode, highlighting its role in real-time data integration and communication.
      
   3. Main objective

      * Develop a Java application: Create a Java application that integrates Apache Kafka in KRaft mode.
      * Enable message communication: Establish seamless message sending and receiving between two PCs using Kafka.
      * Configure Apache Kafka: Set up and configure Kafka for KRaft mode to ensure proper functioning without Zookeeper.
      * Implement producer and consumer: Develop a Kafka producer to send API data messages and a Kafka consumer to receive and display these messages.
      * Demonstrate real-time data processing: Showcase the application’s ability to handle real-time data streams across distributed systems.
      * Document and present: Create comprehensive documentation, an architecture diagram, and a video presentation to demonstrate the system’s setup and functionality.
        
   4. Methodology

      To begin with, we set up Apache Kafka in KRaft mode by downloading the latest version from the official website and extracting it on both PCs. We then modified the server.properties file to enable KRaft mode, ensuring the cluster ID was set and removing the Zookeeper settings. We also made sure that the Kafka ports were open and accessible between the two PCs. Using the Kafka scripts, we started the Kafka broker on both PCs and verified their communication.

      Next, we developed the Java application. On PC 1, we set up a new project in IntelliJ IDEA, included the Kafka client library via Maven dependency, and created a Producer class. This class was designed to send messages containing API data to a predefined Kafka topic. Simultaneously, on PC 2, we set up another Java project and created a Consumer class. This class subscribes to the same Kafka topic to read and display messages, thus validating successful communication between the two systems.

      For testing and validation, we ensured that the Kafka servers on both PCs could communicate effectively.
   9. Result
   10. Conclusion

## Architecture Diagram
## References (Not less than 10)
## Youtube Presentation
## Result/Output (Screenshot of the output)

