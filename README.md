## Requirements for Assignment #2
[Read the instruction](https://github.com/STIWK3014-A241/class-activity-stiwk3014-class-activity-team/blob/main/Assignment-2.md)

## Assessment Criteria
[Check the rubrics](https://github.com/STIWK3014-A241/class-activity-stiwk3014-class-activity-team/blob/main/Rubrics-Assignment-2.md)

## Your Info:
1. Matric Number & Name & Photo & Phone Number
2. Other related info (if any)

|    |                          NAME                            |           MATRIC NUMBER          |              PHONE NUMBER | PICTURE           |
| -- | -------------------------------------------------------- | -------------------------------- | --------------------------------------------- | ------- |
| 1. | <div align="center">MUHAMMAD DANIAL BIN MOHD FARIS</div> | <div align="center">294692</div> | <div align="center">(+60) 12 - 451 6452</div> | <div align="center"><img src="https://github.com/user-attachments/assets/13415d47-f128-427e-842d-fc8b3a27a858" alt="MUHAMMAD DANIAL BIN MOHD FARIS (294692)" width="100px"></div> |
| 2. | <div align="center">SHARWIN A/L PARAMESWARAN</div>       | <div align="center">295026</div> | <div align="center">(+60) 12 - 647 1786</div> | <div align="center"><img src="https://github.com/user-attachments/assets/8ef08b3b-4ea3-4b53-88fb-fcddd9eb182a" alt="SHARWIN A/L PARAMESWARAN (295026)" width="100px"></div> |

## Title: Real-Time Messaging with Apache Kafka in KRaft Mode
## Abstract (in 300 words)
   1. Background

      Apache Kafka is a powerful distributed messaging platform used for building real-time data pipelines. Traditionally, Kafka relied on Apache ZooKeeper for managing clusters, but with the introduction of KRaft mode, Kafka now handles cluster management itself, improving scalability and simplifying architecture. This assignment focuses on setting up Kafka in KRaft mode to create a producer-consumer application, where a Java-based producer sends data from a quotes API to a consumer over a network. By working with the latest version of Kafka (3.9.0) and KRaft mode, the project provides practical experience in real-time messaging and distributed system architecture.
      
   2. Problem Statement (from article)

      Traditional messaging systems often struggle with real-time data integration due to scalability and latency issues. Apache Kafka addresses these challenges with high throughput, low latency, and fault tolerance, making it ideal for real-time applications (Kreps et al., 2011). This assignment explores Kafka in KRaft mode to showcase its practical role in solving such challenges.
      
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

      For testing and validation, we ensured that the Kafka servers on both PCs could communicate effectively. We tested the Producer on PC 1 by sending API data messages and validated the Consumer on PC 2 by receiving and displaying these messages.

      In terms of documentation and presentation, we documented the setup process, created an architecture diagram, and recorded the results in a comprehensive Readme.md file. We included screenshots of the results, and recorded a video presentation of the system implementation. This video was uploaded to YouTube and the link was included in the documentation.

      Lastly, we compiled a list of at least 10 references used during the project and uploaded all source codes to the designated GitHub repository. We ensured that all images and resources were correctly included in the project to complete the submission.
      
   5. Result

      The assignment successfully showcased the configuration and implementation of Apache Kafka in KRaft mode for real-time messaging between two PCs. Using the Quotes API from API Ninjas, the Java-based Producer on PC 1 fetched a random quote and sent it to a Kafka topic. The Consumer on PC 2 subscribed to the same Kafka topic, receiving and displaying the random quote accurately, thus validating seamless communication. The Kafka servers on both PCs communicated effectively, highlighting Kafka's capability in handling real-time data streams. The system's setup, architecture, and functionality were well-documented, with detailed screenshots and a comprehensive video presentation, fulfilling all the assignment requirements.
      
   6. Conclusion

      In conclusion, this assignment provided a practical understanding of configuring and using Apache Kafka in KRaft mode for real-time messaging between two PCs. Through the development of a Java-based Producer and Consumer, we successfully demonstrated efficient message communication, highlighting Kafka's capabilities in handling real-time data integration. The hands-on experience reinforced our knowledge of distributed system architecture and the critical role of Apache Kafka in modern data processing environments.

## Architecture Diagram
![architectural diagram](https://github.com/user-attachments/assets/29236558-df34-4774-9f09-850c71d261f9)

## References (Not less than 10)

   1. Apache Kafka. (n.d.). Apache Kafka. https://kafka.apache.org/
   2. KRaft - Apache Kafka without ZooKeeper. (n.d.). Confluent. https://developer.confluent.io/learn/kraft/
   3. KRAFT Overview | Confluent Documentation. (n.d.). https://docs.confluent.io/platform/current/kafka-metadata/kraft.html
   4. Getting Started with the KRaft Protocol | Confluent What is KRaft, and how to get started. (n.d.). Confluent. https://www.confluent.io/blog/what-is-kraft-and-how-do-you-use-it/
   5. Instaclustr. (2022, November 22). Apache Kafka® KRaft Abandons the Zoo(Keeper): Part 1 — Partitions and data performance. Medium. https://instaclustr.medium.com/apache-kafka-kraft-abandons-the-zoo-keeper-part-1-partitions-and-data-performance-5b0af26184ca
   6. Apache Kafka. (n.d.-b). Apache Kafka. https://kafka.apache.org/20/documentation.html
   7. The basic Kafka. (n.d.). Google Books. https://books.google.com.my/books?hl=en&lr=&id=q71jhLcPd8gC&oi=fnd&pg=PR9&dq=kafka&ots=i2QgQT5pmZ&sig=o0Pfj5VCL8w3Zje0D5wIIBZ8Cs0&redir_esc=y#v=onepage&q=kafka&f=false
   8. Kreps, J., Corp, L., Narkhede, N., & Rao, J. (n.d.). Kafka: a Distributed Messaging System for Log Processing. https://pages.cs.wisc.edu/~akella/CS744/F17/838-CloudPapers/Kafka.pdf
   9. Helenius, S. (2024, August 19). Performance evaluation of Apache Kafka and RedPanda. https://aaltodoc.aalto.fi/items/3e46a100-f126-4880-91e4-4389a9c2efdb
   10. Kafka in action. (n.d.). Google Books. https://books.google.com.my/books?hl=en&lr=&id=jehZEAAAQBAJ&oi=fnd&pg=PA1&dq=apache+kafka+kraft&ots=A-TTmFQJLA&sig=kppICS8szmV9-ZeHtEaQe-MKRE8&redir_esc=y#v=onepage&q=apache%20kafka%20kraft&f=false
   11. Povzner, A., Mahajan, P., Gustafson, J., Rao, J., Juma, I., Min, F., Sridharan, S., Bhatia, N., Attaluri, G., Chandra, A., Kozlovski, S., Sivaram, R., Bradstreet, L., Barrett, B., Shah, D., Jacot, D., Arthur, D., Dagostino, R., McCabe, C., . . . Gupta, K. (2023). Kora: A Cloud-Native event streaming platform for Kafka. Proceedings of the VLDB Endowment, 16(12), 3822–3834. https://doi.org/10.14778/3611540.3611567
   12. Jones, W. (n.d.). Standardizing Data For Kafka Consumers. Retrieved December 14, 2024, from https://iamwpj.com/papers/Standardizing%20Data%20For%20Kafka%20Consumers.pdf
   13. Gilles Deleuze, & Félix Guattari. (2016). Kafka: Toward a Minor Literature. University Of Minnesota Press. https://complit.utoronto.ca/wp-content/uploads/COL1000-Week02-September23_GillesDeleuzeFelixGuattari.pdf

## Youtube Presentation
## Result/Output (Screenshot of the output)

Producer (PC1) :

![image](https://github.com/user-attachments/assets/dacd9fb7-0326-4b44-bc9d-b38122d27831)


Consumer (PC2) : 

![image](https://github.com/user-attachments/assets/81c8d26f-e662-4a79-9bd8-44866d917368)

