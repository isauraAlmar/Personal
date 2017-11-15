# 

# Fial Project

## INTRODUCTION

### About the company

Everis an NTT DATA Company is a multinational consulting firm that offers business and strategic solutions, development and maintenance of technological applications and outsourcing services. The company, which operates in the telecommunications, financial, industrial, utilities, energy, public administrations and health sectors, reported 1.03 billion Euro in turnover last year. It currently employs 19,000 professionals at its offices and high performance centers in 16 countries.

Everis NTT DATA:
In October 1996 in Spain, a group of entrepreneurs you could count on the fingers of one hand left their managerial positions at a leading consulting company to create a new concept of consulting. The idea was simple to explain, yet complex to implement: build from scratch a unique company model designed to attract and retain the best talent, while fostering good people and collective values. Our talent management model, the main asset of Everis, is taught as a case study in leading business schools, as it excels in smartly feeding both the brain (skills and professional growth) and the heart (attitudes and values) of our employees. The result is summarized in our claim: attitude makes the difference.

From early days in Spain, Everis has grown organically, in double digits. Currently, Everis pass from 5 employees back in 1996 to more than 16,000 across 16 countries and 4 continents.

IMAGE OF NEXTGEN AREA

 
 * Everis NEXT:
 * Aumented workforce:
 Artificial intelligence & Robotics:
The main goal of the team at Everis is to integrate the robots into the society to generate a global benefit. Instead of focusing on the robot, the main goal of the company is the relation between human-robot in order to generate a smooth and friendly interaction. 

We have two areas of actuation:
Business (non-industrial) where through introducing robots in companies the workers will feel more comfortable. 
Social focusing on using the robotics to improve the society. For example, people with disabilities, improve learning or robot partner.

* CLOQQ

* EVERIS INFINITE

### Problem Definition

## THERORY

### RELATIONAL vs NoSQL 


#### Limitations of Relational Databases
Nowadays the amount of data that needs to store and the process has been increasing in big quantities. The way of supporting large numbers of users from companies like Google, Facebook, Amazon, etc. were much different than from supporting much smaller numbers of business users. The way to scale the amount of that in the pass was by Scale up (upgraded with more CPUs, additional memory, or faster storage devices). Scaling up is always a cost concern, and you always are restricted for the hardware capacity. Another option is to use multiple servers but managing a relational DB using different servers increase the complexity and the difficulty

Web applications serving tens of thousands or more users were difficult to implement with relational databases. Four characteristics of data management systems that are particularly important for large-scale    data management tasks are:

* Scalability

* Cost

* Flexibility

* Availability


### NoSQL types 
* Column Families: 

Advantages
Most of the solutions, such as Apache Cassandra, HBase, and Google Datastore, allow adding columns over time without having to worry about filling in default values for the existing rows for the new columns. This gives flexibility in model and entity design allowing one to account for new columns in future for unforeseen scenarios and new requirements.

There are advantages when working with a subset of the available columns. For example, computing maxima, minima, averages and sums, specifically on large datasets, is where these column-oriented data stores outshine in performance. Similarly, when new values are applied for either all rows at once or with same-column filters, these databases will allow partial data access without touching unrelated columns and be much faster in execution.

* Document Store

A document store allows the inserting, retrieving, and manipulating of semi-structured data. Most of the  databases available under this category use XML, JSON, with data access typically over HTTP protocol using RESTful API

Document-oriented databases provide this flexibility—dynamic or changeable schema or even schemaless documents. Because of the limitless flexibility provided in this model, this is one of the more popular models implemented and used. Some of popular databases that provide document-oriented storage include:
* MongoDB

* CouchDB

* Jackrabbit

* Lotus Notes

• Apache Cassandra

• Terrastore

• Redis

• BaseX

Advantages
The most prominent advantage, as evident in the preceding examples, is that 
content is schemaless, or at best loosely defined. This is very useful in web-based 
applications where there is a need for storing different types of content that may 
evolve over time. For example, for a grocery store, information about the users, 
inventory and orders can be stored as simple JSON or XML documents. Note that 
"document store" is not the same as "blob store" where the data cannot be indexed.
Based on the implementation, it may or may not be possible to retrieve or update a 
record partially. If it is possible to do so, there is a great advantage. Note that stores 
based on XML, BSON, JSON, and YAML would typically support this. XML-based 
BaseX can be really powerful, while integrating multiple systems working with XML 
given that it supports XQuery 3.0 and XSLT 2.0.
Searching across multiple entity types is far more trivial compared to doing so in 
traditional RDBMS or even in column-oriented databases. Because, now, there is no 
concept of tables—which is essentially nothing more than a schema definition—one 
can query across the records, irrespective of the underlying content or schema or in 
other words, the query is directly against the entire database. Note that the databases 
allow for the creation of indexes (using common parameters or otherwise and evolve 
over time).
JSON-based stores are easy to define what I call 
projections. Each top-level key 
for the JSON object may be the entity's projection across other parts of the system 
thereby allowing the schema to evolve over time with backward compatibilit

* Key Value

* Graph Databases

* Multimodel Databases

##### Michroservices 

##### Container

##### CAP Therorem

Also known as Brewer’s theorem states that distributed databases cannot have concistenci Availability and Partitiob Tolerance all at the ssame time.

* Consistency: consistent copies of data on different servers.

* Availability: refers	to providing a response	to any query

* Partition Tolerance: 	means if a network that connects two or	more data ase servers fails, the servers will still be	available with consistent data.

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
### Tecnologies

#### Cassandra:
Apache Cassandra is open source, distributed data storage system that differs sharply from relational database management systems.

##### The History of Cassandra

Cassandra first started as an incubation project at Apache in January of 2009. Shortly thereafter, the committers, led by Apache Cassandra Project Chair Jonathan Ellis, re-leased version 0.3 of Cassandra, and have steadily made minor releases since that time.

Though as of this writing it has not yet reached a 1.0 release, Cassandra is being used in production by some of the biggest properties on the Web, including Facebook,Twitter, Cisco, Rackspace, Digg, Cloudkick, Reddit, and more.

Releases after graduation include:

    0.6, released Apr 12 2010, added support for integrated caching, and Apache Hadoop MapReduce
    0.7, released Jan 08 2011, added secondary indexes and online schema changes
    0.8, released Jun 2 2011, added the Cassandra Query Language (CQL), self-tuning memtables, and support for zero-downtime upgrades
    1.0, released Oct 17 2011, added integrated compression, leveled compaction, and improved read performance
    1.1, released Apr 23 2012, added self-tuning caches, row-level isolation, and support for mixed ssd/spinning disk deployments
    1.2, released Jan 2 2013, added clustering across virtual nodes, inter-node communication, atomic batches, and request tracing
    2.0, released Sep 4 2013, added lightweight transactions (based on the Paxos consensus protocol), triggers, improved compactions, CQL paging support, prepared statement support, SELECT column alias support

##### Why Cassandra

* Is highly scalable

* Write Speed: 

* It provides high availability

* Designed to manage very large amounts of structured data like logs.

* It provides high availability

* Peer-to-peer distribution model. 

* The gossiper is a protocol communication (to support decentralization and partition tolerance) responsible for making sure every node in the system eventually knows important information about every other node's state, including those that are unreachable or not yet in the cluster when any given state change occurs. 

* It have AntiEntropy,  it is a synchronization mechanisme that consist in comparing all the replicas of each piece of data that exist (or are supposed to) and updating each replica to the newest version. 

* CQL (Cassandra Query Language), it is a subsed of SQL and its easy for someone coming from SQL to learn. 


#### ElasticSerch
Elasticsearch is a a distributed search engine base on RESTful, capable of solving a growing number of use cases. 
##### History

Elasticsearch had the first vertion realise created for Shay Banon in Febrary 2010. Shay Banon had a scalability isure with Compass and he decide to rewrite and used a common interface, JSON over HTTP, suitable for programming languages other than Java as well.

##### Why Elastic serch

* SPEED: It is really fast. 

* SCALABILITY: 

* Resilient, Highly Available

* CLIENT LIBRARYES: curl, java, c#, python, javascrip, perl, PHP, ruby

* X-PACK: Extend Elasticsearch with Powerful pluguings like BigDesk, Head, HQ, Kopf, and Paramedic.

#### Docker

##### History
##### Characteristics
##### Why Docker

* Portability: Everything required to run the application is packaged into a standardized container which means your applications are no longer restrained to certain infrastructure requirements. Applications can move across multiple environments, development stages, and cloud environments - consistently.

* Incrise security: The Docker EE platform provides you with all the tools and capabilities you need to run containers securely at scale. With services like security scanning and container signing, Docker EE enables you to protect all app components from the source, across the network, and to different collaborators and environments with guarantees against tampering.

* Efficiency: By containerizing your legacy application on Docker Enterprise Edition (EE), you reduce the total resource requirements to run your application. This increases operational efficiency and allows you to consolidate your infrastructure.





#### Elisandra = Elasticserch + Casandra
![alt text](https://github.com/isauraAlmar/Personal/blob/master/elassandraarchitecture.jpg)
##### History
##### Characteristics
##### Why Elassandra

### Schedule

A gantt diagram

## Solution
## Reflections
## Conlutions
 
