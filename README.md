# Final Project

## INTRODUCTION

The goal of this chapter is to provide context about the environment where this project has been developed. The first subsection will provide a general overview of the project, explaining the antecedents and the original idea.

As the project has been developed in collaboration with a company, the second subsection will include some background information about the company, everis

The next part dives deeper into the structure of everis, and will focus on NextGen, everis innovation area. The fourth subsection will explain the structure of the Robotics/Augmented Workforce team, where I am currently working. We will finish this part explaining the current needs of the different projects in which my team is working, and how this project is able to help.

### Project overview

Robots are becoming increasingly present in everyday's life, and are an active area of research, where the theoretical applications are almost infinite. However, the most interesting and powerful features, usually involve processing a real-time stream audio or video stream, in search of different patterns: such as words, objects, faces, movements... and then use machine-learning to generate a customised response, while having several other threads running. This requires a high computing power, and processing and storing big quantities of data.

As most of them do not have a significant computing power, this is a challenge that must be solved in order to improve the capabilities of current robots. There are several reasons for this hardware limitation. Sometimes, a better chip simply doesn't fit into the available physical space on the robot without changing the design, other times a customised chip would be needed, increasing vastly the costs of mass-production of the robots, and also sometimes it is caused by robot designers, who did not think on that possible use of the robot. There are, of course, some high-end robots whose hardware is not that constraining, but their prices are usually very high, so few consumers have access to them.

That is why in my team came up with the idea of creating a server for the robot to connect, and send information about the state of the sensors and actuators. The server doesn't have the same hardware constrains, so it could compute them and send the processed data to the robot, so its role would only be performing the computed response. Furthermore, if instead of only a server, you use “the cloud”, you can have as much computing power and storage as needed, with the only requirement of having internet access. This would also open the door to have different robots connected to the cloud, sharing a common "knowledge base", and allowing application developers to invent brand new ways of exploiting this common information.

The combination of different trending technologies such as big data, cloud computing, machine-learning and robotics can lead to a significant advance in the field. Let's imagine that a girl named Lisa, enters into a department store for the first time. At the entrance, she meets a robot, who learns her name and her face, and with the help of the wireless cameras and NFC sensors, analyses the behaviour of Lisa, learning about what she purchased and what she didn't. If any other day Lisa decides to go to another store of the same brand, their local robot already knows who she is, her interests last time, and a record of what she purchased in the past, so he can greet her "Hey Lisa, do you remember the jacket you tried on your last visit? Today you can buy it with a -40% discount!".

So this is where this project comes. The main goal is to generate a simple, yet scalable, proof of concept system which should allow robots to send data to process and receive a processed output, and allowing a second robot to access the knowledge generated by the first one. On the educational side, this project will allow me to investigate different technologies, and design the architecture of a complex cloud-based system, while allowing different robots to interact with it.


### About the company

everis, an NTT Data Company, is a multinational consulting firm that offers business and strategic solutions, development and maintenance of technological applications and outsourcing services. The company has grown organically, in double digits and reported 1.03 billion Euro in turnover last year. It currently employs more than 20,000 professionals at its offices and high-performance centres, located in 16 countries. Its main operation areas are Western Europe and Latin America.

The company was originally named DMR Consulting and was founded in Spain on October 1996, when a group of 5 entrepreneurs left their managerial positions at a leading consulting company to create a new concept of consulting. The idea was simple to explain, but complex to implement: building from scratch a unique company model designed to attract and retain the best talent, while fostering good people and collective values. Our talent management model, the main asset of everis, is taught as a case study in leading business schools, as it excels in smartly feeding both the brain (skills and professional growth) and the heart (attitudes and values) of our employees. The result is summarised in our claim: attitude makes the difference.

What Everis can do for companies:

* Disruption, why go far if you can go further

* Consulting, successful Digital projects with Everis

* Transformation we define pragmatic and realistic initiatives, making transformation happen.

* Technology, we provide the best technology and enterprise solutions to create new experiences.

* Operations, Delivering quality and efficient Managed Services


### About the department
![alt text](https://github.com/isauraAlmar/Personal/blob/master/NexGenScema.png)


 * Everis NEXT:

 * Augmented workforce:
 Artificial intelligence & Robotics:
The main goal of the team at Everis is to integrate the robots into the society to generate a global benefit. Instead of focusing on the robot, the main goal of the company is the relation between human-robot in order to generate a smooth and friendly interaction.

We have two areas of actuation:
Business (non-industrial) where through introducing robots in companies the workers will feel more comfortable.
Social focusing on using the robotics to improve the society. For example, people with disabilities, improve learning or robot partner.

* CLOQQ: CLOQQ (acronym for "Crea Lo Que Quieras" in English  "Create What You Want") offers both face-to-face activities (workshops, events, etc.) and a complete online and content environment for girls and boys to create their own video games, apps, robots, animations and much more. Watch video.

https://www.everis.com/spain/es/news/newsroom/everis-lanza-cloqq-una-iniciativa-para-que-ninos-y-ninas-se-diviertan-aprendiendo-0

* EVERIS INFINITE:  Everis Infinite is a free software application from the Office Suites & Tools subcategory, part of the Business category. The app is currently available in English and it was last updated on 2017-01-20. The program can be installed on iOS.
https://everis-infinite-ios.soft112.com/

### About the team

Artificial intelligence & Robotics:
The main goal of the team at Everis is to integrate the robots into the society to generate a global benefit. Instead of focusing on the robot, the main goal of the company is the relation between human-robot in order to generate a smooth and friendly interaction.

We have two areas of actuation:
Business (non-industrial) where through introducing robots in companies the workers will feel more comfortable.
Social focusing on using the robotics to improve the society. For example, people with disabilities, improve learning or robot partner.

Robots that the team works with:

###### Pepper
Pepper is a robot from Aldebaran, a partner of Soft Bank Group. It is a humanoid robot that is 1,20 meters tall, and it is created to interact with it in different ways like having a vocal interaction, through its tablet, it has different sensors, etc.


###### Jibo
###### Tiago
###### Nao
###### Pleo and Casper project
###### Sota


### Problem Definition // TODO: Adapt
Robotics found that some of the robots do not have a significant computing power that is a problem when you need to have a few different processes running at the same time, especially when those processes have a big amount of data like processes that use image processing or machine learning. (CONECTOR) there exist robots that can handle high processing costs, but they usually are very expensive.

That is why the team had the idea about creating a server where the robot will connect to it and send information about the state of the sensors and actuators. The server will compute them and send the data to the robot about what they have to do. Furthermore, if you pout that server in “the cloud”, you can connect the robots and connect any robot from everywhere, with the only requirement of having internet access. Also if you have different robots connect to the cloud, you have the possibility of shearing the knowledge between robots. A here is where this project comes. The idea is to create a proof of concept of a system where tow robots that connect to it can share information.

Imagine that a girl called Lisa, enters into a store for the first time. At the entrance, she meets a robot, and the robot learns who she is, and . Another day Lisa go to another store with the same company as before that is located in another city. There is also a robot, and it already knows who Lisa is, her interests last time, and a record of what she pushes in the past.

In conclusion, the purpose of this project is double. One the one hand, it aims to investigate and design a system where robots can connect to get enhanced capabilities. On the other hand is to develop the data model where this knowledge adquired by the robots will be stored.

Nowadays, every company is e alot the word of BigData. One need that the company have is to be able to store all the interactions betwen the robots and the persons in order to analyse them. So the system has to be able to save all the logs in the database.


The previous example shows in big words what the system have to do.
(CREAT IT)

### What they have

Before I start the project the companye had a small Proof of Concept (PoC). This PoC is built around two docker containers:

* One call streaming that.

* Another one

##### ROS Requirements

### Requisites

The system needs to be prepared for scalability in two ways:

* The fist one it refers the number of robots. We will be able to have at least 1 robot at the beginning. But in about a year it is expect to have connect in it around one million of robots. So it is important that there is no problem on adding robot very fast.

* The second one it refers on the software side. The system need to be able to add functionalities in a easy way. An example of functionality may be face detection, Neurolinguistic programming, mapping, a new behaviour, etc.

Another challenge that the system needs to overcome is the fact of being multiplatform. It needs to be able to communicate with robots of many brands. On the other way also it requires integrating behaviours and functionalities than can be code in multiple languages or run in a separate different OS.  

When you are talking about social robots it is important to mention real time interactions, that is the reason why the system needs to be able to have streaming communication.

### Propose of the project
(INSTEAD OF MENTIONING I SHOULD EXPLAIN THEM)

Why SQL or NoSQL? Which can be a good database for saving the logs and all the knowledge?

Which system, is ROS scalable enough, does it accomplish all our needs?

Which type of Architecture is the best for The cloud system?

## Analysis and reserch

These section is about taking the needs of the project learning the theory that is related with it and research about which technologies can be use and which ones may work better.


### Big picture of the system.

( ESQUEMA SIN HABLAR DE TECNOLOGIAS SOLO CON ELEMENTOS )

### Database
( BREVE INTRODUCCION )


##### CAP Theorem

Also known as Brewer’s theorem states that distributed databases cannot have consistency Availability and Partition Tolerance all at the same time.

* Consistency: consistent copies of data on different servers.

* Availability: refers to providing a response to any query

* Partition Tolerance: means if a network that connects two or more databases and if one servers fails, the servers will still be one available with consistent data.

#### Relational vs NoSQL

##### Limitations of Relational Databases
Nowadays the amount of data that needs to be stored and the processed has been increasing in big quantities, and with it new terms have come such as "BIG DATA", "Internet of Things" or "Analytics". The way of supporting large numbers of users from companies like Google, Facebook, Amazon, etc. change the way of managing data than smaller numbers of business users.  

Web applications serving tens of thousands or more users were difficult to implement with relational databases. Four characteristics of data management systems that are particularly important for large-scale data management tasks are:

* Scalability: The way to scale the amount of that in the pass was by Scale up (upgraded with more CPUs, additional memory, or faster storage devices). Scaling up is always a cost concern, and you always are restricted for the hardware capacity. Another option is to use multiple servers but managing a relational DB using different servers increase the complexity and the difficulty.

* Cost: Upgrading with better hardware always have a huge impact of cost ??????

* Flexibility:   

* Availability: Being able to querying is one of the big problems when you have millions of users accessing the information at almost the same time from anywhere in the world. We need to ensure that the database has a way to ensure that the data when there are infrastructure problems, or system errors. With Relational Databases is not an easy problem to solve, it can become a very complicated problem when maximises the availability is needed.  

##### NoSQL

The idea of the NoSQL database is to solve the problems that the typical relational database has. A good definition for a NoSQL is a variety of different database technologies that are being non-relational as we mentioned before that is one of the problems that we are having with very large amount of Data, it is also distributed meaning that they can be inculcate to multiple processors. Another characteristic of the NoSQL is that they have to be horizontally scalable, that means that we can increase the number of the nodes, and not having to scale vertically, increase the size of the node.

!!DRAW OF VERTICAL AN HORITZONTAL scaling.


When we talk about big data we have 4 dimensions or the 4 V:   

* Volume: It refers the amount of data. We have many sources that the data can be generated form. For exemple: Logs, senors, social media, speeach, events, etc.

* Variety: It refers the types of data that we can have. It can be structured, semi-structured or unstructured. The data can come from two main sources: people who create the data and or machines. In the case of the people it is going to be more structure. And in the case of machines it depends.

* Veracity: How truthy is the data. In some cases, we can have untrusted data, for example if you have a node replicated many times and the data it is not consistent between them.

* Velocity: The velocity that we need to process the data either the speed of generating (and saving) the data and the read of analysis.  
https://bicorner.com/2015/06/25/characteristics-that-make-big-data-big/ (1/12/2017)

##### Types of NoSQL

* Column Families:

These types of Database are designed to manage big amount of data distributed on multiple servers in a cluster. If you only have one server probably these type of data is not what you need.

EXPLAIN HOW IT WORKS

* Document Store

A document store allows the inserting, retrieving, and manipulating of semi-structured data. Most of the databases available under this category use XML, JSON, with data access typically over HTTP protocol using RESTful API

Document-oriented databases provide this flexibility—dynamic or changeable schema or even schemless documents. Because of the limitless flexibility provided in this model, this is one of the more popular models implemented and used. Some of popular databases that provide document-oriented storage include:


* Key Value

When we talk about key value database we need to imagine an array that have constrains on the keys and the values. That king of array is what we call associative array. The advantages that you can have on a key value database over an associative array is the persistence of the data especially in long term storage.

The idea of a key value is to be able to the fast access of the data, that is the reason why some key value stores only use memory to keep the data instead of saving it into the disk.  

It is good to implement these kinds of database when you need to use many times a data, so when we get it form the disk it saves the data to the cache in order to access it faster.

* Graph Databases

Graph Databases as its name suggest, is a database base on the mathematical element name graph. A graph consists on two parts, vertices and edges, where a Vertices represents thinks (it can be anything, cities, animals, stations, etc.) that have relationships with other thinks. On the other hand, edges are the links that connect vertices and represents its relationships. The relationships can be long or short term.

* Multimodal Databases

Sometimes one type of database it does not required all the characteristics of the system. Sometimes is good to combine the different models for a better performance. For example, when a user logs into the system it might need to access the data of the user many times, a good possibility for having better speed is to use a SQL database that needs to be done  

#### Table of compatating technologies

| Tecnology |type | Advantage | disadvantages  |
| ---------------- |:--------------------|:-----------------------------------:|:-----------------------------------:|
| Apache Cassandra | column store      | open source. Per to per architecture. Scheme free. | $1600                    |
| MongoDB          | document store | Schema less |            $12                            |
| ArangoDB           | Multimodal Database |                          w               |                    $1 |
| Hadoop           | Colum store    |Open source It can manage multiple nodes acros different servers working in parallel. It is good to manage large numbers of unstructured data. It is fault tolerance | Security: No data encryption. Limitations at the time to improve efficiency, reliability and integration|
| Couch DB         | document store |                         w                |                   w                      |
| Elastic          |          w     | or Azure SQL Database                   |                   w                      |

I will explain the tecnologye I had use and the reason at ROJECT DEVELOPMENT section

### Architecture
(SHORT INTRODUCCTION)

#### SOA
#### Microservices  
" Self contained process that provides a unique business capability"
https://www.youtube.com/watch?v=PY9xSykods4

it is important to focus on single business capabilities.
* almost dtateles of the aplication

IMPORTANT SETTINGS

each group need to have ouw data model.
make communication state less

REAL EXAMPLES:
* Amazon

Advantages:

* It is easy to have small teams developing each capability
* Incase that one service broke the others will keep working



##### ACID:
*Atomicity: A unit that cannot be further divided.

*Consistency: Ensure the integration of data.

*Isolation:

*Durability:

##### BASE:

*Basically:

*Available:

*Soft State:

*Eventually Consistent:

## PROJECT DEVELOPMENT

### Introduction

In this section It describes the research about which technologies that can be used to solve the database problem, and a comparison between them to find which ones can be the best. It is also to define the architecture of the system and which technologies that can be used to implement it.  

### Technologies

#### Tecnologies for Database

For crating a database I use Elasandrea, that is a convertion fo Cassandra, an NoSql using the colum family model, and Elastic search a serche engine.

##### Cassandra:
Apache Cassandra is open source, distributed data storage system that differs sharply from relational database management systems.

Cassandra is a NoSQL using Column Store model. It has a primary language call CQL (Cassandra Query Language) that is use for communicating with the database.  

![alt text](https://github.com/isauraAlmar/Personal/blob/master/Screenshot from 2017-12-04 15-50-51.png)

##### The History of Cassandra

Cassandra first started as an incubation project at Apache in January of 2009. Shortly thereafter, the committers, led by Apache Cassandra Project Chair Jonathan Ellis, re-leased version 0.3 of Cassandra, and have steadily made minor releases since that time.

Though as of this writing it has not yet reached a 1.0 release, Cassandra is being used in production by some of the biggest properties on the Web, including Facebook, Twitter, Cisco, Rackspace, Digg, Cloud kick, Reddit, and more. \[book]

Releases after graduation include:

    0.6, released Apr 12 2010, added support for integrated caching, and Apache Hadoop MapReduce
    0.7, released Jan 08 2011, added secondary indexes and online schema changes
    0.8, released Jun 2 2011, added the Cassandra Query Language (CQL), self-tuning memtables, and support for zero-downtime upgrades
    1.0, released Oct 17 2011, added integrated compression, leveled compaction, and improved read performance
    1.1, released Apr 23 2012, added self-tuning caches, row-level isolation, and support for mixed ssd/spinning disk deployments
    1.2, released Jan 2 2013, added clustering across virtual nodes, inter-node communication, atomic batches, and request tracing
    2.0, released Sep 4 2013, added lightweight transactions (based on the Paxos consensus protocol), triggers, improved compactions, CQL paging support, prepared statement support, SELECT column alias support

##### Why Cassandra
* Scalability: In the system is very important to design for a scalability because the company could decide to add hundreds of new robots over a short period of time. So, Cassandra is prepared to have a high scalability performance.  

* Write Speed: It is important that when the system want to save new information it does fast because there may be vast amounts of information to save. One of the examples that needs to be fast is when you save all the interaction information as a log.

* It provides high availability:  

* Designed to manage very large amounts of structured data like logs.

* Peer-to-peer distribution model.  

* The gossiper is a protocol communication (to support decentralisation and partition tolerance) responsible for making sure every node in the system eventually knows important information about every other node's state, including those that are unreachable or not yet in the cluster when any given state change occurs.  

* It have AntiEntropy,  it is a synchronisation mechanism that consist in comparing all the replicas of each piece of data that exist (or are supposed to) and updating each replica to the newest version.  

* It use CQL (Cassandra Query Language), it is a subset of SQL and its easy for someone coming from SQL to learn.  
##### Requirements

* minimum 2 cores, recommended 8 or more cores.
* minimum 8GB of RAM, recommended 32GB of RAM.
* Java 8
* Python 2.7

#### Elasticsearch

Elasticsearch is a search engine base on RESTful, that have two main functions: it can be used as an analytic framework and datastore as well.

It can be used for several cases:  
* As a Text Search.
* Event Data and Metrics.
* Visualising Data.
* Scraping and Combining Public Data.
* Logging and Log Analysis.


  (HERE I HAVE TO EXPLAIN THAT IS DOCUMENT BASE)

##### History

Elasticsearch had the first version released for Shay Banon in Febrary 2010. Shay Banon had a scalability issue with Compass and he decide to rewrite and used a common interface, JSON over HTTP, suitable for programming languages other than Java as well.

##### Why Elasticsearch

One of the advantages of Elasticsearch is that you can create a client made of any language as the answer is a JSON object. The main advantages of these protocol are:

* Portability: It use web standards so it can be implemented in many languages such as Java, Python, Ruby, c#, etc., or called form command lines applications such as curl.

* Durability:

* Simple to use:

* Speed: It can compute complex queries in a short amount of time.

* High support: A lot of plugins uses a REST endpoint on HTTP.

* Scalability:  Is the same to talk to Elasticsearch running on a single node than hundreds of them. It scales horizontally to handle billions of events per second, while automatically managing how indices and queries are distributed across the cluster for oh-so smooth operations.

* Security: Elasticsearch out of the box it does not have than hight up security control. It use HTTP authentification. But as I mention before there are lots of plugins, for example SearchGuard is a free plugin that you can find role based access control, document level security and SSL/TLS encrypted node-to-node communication. You can also find other pluging for security.

* It has a big community that maintain and use it. That can be really useful at the time to solve problems or learn how to use it. Another reason is because the community apart official rivers that support the most use programming languages.


* Resilient, Highly Available

##### Requierments
 * Java 8
 * curl

#### Elassandra = Elasticsearch + Cassandra

"Elassandra is a fork of Elasticsearch modified to run as a plugin for Apache Cassandra in a scalable and resilient peer-to-peer architecture. Elasticsearch code is embedded in Cassandra nodes providing advanced search features on Cassandra tables and Cassandra serve as an Elasticsearch data and configuration store. "

https://github.com/strapdata/elassandra

![alt text](https://github.com/isauraAlmar/Personal/blob/master/elassandraarchitecture.jpg)
  https://github.com/strapdata/elassandra

##### History
##### Characteristics
##### Why Elassandra

* It have an enterprise version, Strapdata
* An Elasticsearch index is mapped to a cassandra keyspace, and a document type to a cassandra table.
* Docker
* Durability
* CQL (Common Query Language): it is possible to perform CQL queries to .
* It is possible to use the plugins of Elasticsearch.
* Definitely it has the advantages of Elasticsearch and cassandra all together.

##### Requirements
* Java 8


### Technologies for the architecture

#### Docker
Docker is a container technology that is create
##### History
##### Characteristics
##### Why Docker

* Portability: Everything required to run the application is packaged into a standardised container which means your applications are no longer restrained to certain infrastructure requirements. Applications can move across multiple environments, development stages, and cloud environments - consistently.

* Increase security: The Docker EE platform provides you with all the tools and capabilities you need to run containers securely at scale. With services like security scanning and container signing, Docker EE enables you to protect all app components from the source, across the network, and to different collaborators and environments with guarantees against tampering.

* Efficiency: By containerising your legacy application on Docker Enterprise Edition (EE), you reduce the total resource requirements to run your application. This increases operational efficiency and allows you to consolidate your infrastructure.

* Enterprise version (EE) and community version (CE)
##### Requirements
* Available for: Mac, Windows, Debian, Ubuntu, CentOS, Azure and AWS.

Depending of the OS. To install Docker CE in Ubuntu, you

* 64-bit version o
* Ubuntu versions: Artful 17.10 (Docker CE 17.11 Edge only), Zesty 17.04, Xenial 16.04 (LTS), Trusty 14.04 (LTS),
* Ubuntu on x86_64, armhf, and s390x (IBM z Systems) architectures.

#### Kafka

![alt text](https://github.com/isauraAlmar/Personal/blob/master/Screen%20Shot%202017-12-11%20at%2012.04.13.png)
##### History  
##### Why kafka
##### Requirements
* Need to have ZooKeeper install and started.
* For ZooKeeper it is need:
	Supported Platforms
		* GNU/Linux.
		* Sun Solaris.
		* FreeBSD.
		* Win32.
		* MacOSX.
	JDK 6 or greater.
*


### Schedule

A Gantt diagram

## Solution
### Architecture design
#### Design for scalability


### Data structure
![alt text](https://github.com/isauraAlmar/Personal/blob/master/cluster.png)

![alt text](https://github.com/isauraAlmar/Personal/blob/master/know-node.png)

People table:

    {
            "pid" : "",      
            "name" : {
                "first_name" : "",
                "last_name" : ""
            },
            "personal_info" : {
                "age" : "",
                "telephone" : "",
                "email" : ""
            },
            "last_seen" : {
            "time_seen" : "",
            "place_seen" : ""
        }
    }

Robot table:

    {
        "rId" : "",
        "rType" : {
            "name" : "",
            "version" : ""
        },
        "rOwner" : ""
    }

Logs interaction table:

    {
        "id" : "",
        "where" : "",
            "network" : "",
            "place" : ""
        },
        "when" : {
            "time" : "",
            "day" : ""
        },
        "info" : {
        }
    }

### Funcionality

## Reflections
## Conlutions

##
### Books


    author name
    title of the publication (and the title of the article if it's a magazine or encyclopedia)
    date of publication
    the place of publication of a book
    the publishing company of a book
    the volume number of a magazine or printed encyclopedia
    the page number(s)

NoSQL for Mere Mortals by Dan Sullivan. Published by Addison-Wesley on April 2015,First printing. Text	printed	inthe	United	States	on recycled paper at Edwards Brothers Malloy, Ann Arbor, Michigan.

Cassandra: The Definitive Guide, by Eben Hewitt, Published by O’Reilly Media on November 2010, First Edition.

Kafka: The Definitive Guide, Real-Time Data and Stream Processing at Scale, by Neha Narkhede, Gwen Shapira, and Todd Palino. Published by O’Reilly Media on July 2017: First Edition.


The OpenCV Tutorials, Release 2.4.13.3, September 03, 2017
### Webs
http://blogs.mindsmapped.com/bigdatahadoop/hadoop-advantages-and-disadvantages/ (1/10/2017)

https://docs.mongodb.com/manual/ (1/10/2017)

https://www.tutorialspoint.com/mongodb/mongodb_advantages.htm (20/11/2012)

https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/ (1/12/2017)

https://www.rosehosting.com/blog/how-to-install-apache-cassandra-on-ubuntu-16-04/ (23/10/2017)

https://docs.datastax.com/en/cql/3.1/cql/cql_intro_c.html (17/10/2017)

##### Elisandra: Elasticsearch + Cassandra
http://doc.elassandra.io/en/latest/installation.html (2/11/2017)

https://github.com/strapdata/elassandra (2/11/2017)

https://www.youtube.com/watch?v=0WuLZTvA3YM (2/11/2017)

##### Elasticsearch

https://www.elastic.co/ (17/10/2017)

https://www.3pillarglobal.com/insights/advantages-of-elastic-search (25/10/2017)
https://apiumhub.com/tech-blog-barcelona/elastic-search-advantages-books/ (11/12/2017)

##### Cassandra

https://docs.datastax.com/en/cql/3.1/index.html (17/10/2017)

##### Kafka

https://kafka.apache.org/documentation/ (10/12/2017)
https://zookeeper.apache.org/doc/r3.1.2/zookeeperAdmin.html#sc_systemReq (11/12/2017)

## Appendix

### Basic concepts
Cluster: a cluster can be a group nodes which can consist of computers, databases, or other techonoglies that work together closely

Node: a single computer or database or techonogly in a system.

Index:

Type:

Document:

Shards and Replicas:

* Container
*
### Abreviations

NoSQL - non relational Structured Query Language

DB - Database

SW - Software

HW - Hardware

OS - Operationg system


//think about the reason behind choosing techonoliges such as documentation, maturity , and the other 3 things

"Kafka Connect currently supports two modes of execution: standalone (single process) and distributed.

In standalone mode all work is performed in a single process. This configuration is simpler to setup and get started with and may be useful in situations where only one worker makes sense (e.g. collecting log files), but it does not benefit from some of the features of Kafka Connect such as fault tolerance. You can start a standalone process with the following command:

1
 > bin/connect-standalone.sh config/connect-standalone.properties connector1.properties [connector2.properties ...]

"
¨
´
" Distributed mode handles automatic balancing of work, allows you to scale up (or down) dynamically, and offers fault tolerance both in the active tasks and for configuration and offset commit data. Execution is very similar to standalone mode:

1
> bin/connect-distributed.sh config/connect-distributed.properties"

" The difference is in the class which is started and the configuration parameters which change how the Kafka Connect process decides where to store configurations, how to assign work, and where to store offsets and task statues. In the distributed mode, Kafka Connect stores the offsets, configs and task statuses in Kafka topics. It is recommended to manually create the topics for offset, configs and statuses in order to achieve the desired the number of partitions and replication factors. If the topics are not yet created when starting Kafka Connect, the topics will be auto created with default number of partitions and replication factor, which may not be best suited for its usage."

Kafka Connect Elasticsearch:

https://github.com/hannesstockner/kafka-connect-elasticsearch (1/12/2017)

Prerequisites:
* a Linux console or Apple OSX console (not tested on windows, but adaptable with little effort)
* a Git client to fetch the project
* Docker Compose
* Apache Maven installed.
* git clone https://github.com/hannesstockner/kafka-connect-elasticsearch kafka-connect-elasticsearch

Kafka Connect Cassandra:

https://github.com/jcustenborder/kafka-connect-cassandra (1/12/2017)

