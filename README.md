# 

# Fial Project

## INTRODUCTION
## THERORY

### RELATIONAL vs NoSQL 


#### Limitations of Relational Databases
Nowadays the amount of data that is need to store and process has been encreasing in big quantities. The way of suporting large numbers of users from companyes like Google, Facebook, Amazon, etc. where much different than from supporting much smaller numbers of business users. The way to scale the amount of thata in the pass was by Scale up (pgraded with more CPUs, additional memory, or faster storage devices). Scaling up is allways a cost concernt, and you are always restric for the harware capacity. Another option is to use multiple servers but managing a relational DB using different servers incres the complexity and the dificulty

Web applications serving tens of thousandsor more users	were difficult	to implement with relational databases. Four haracteristics of data management systems that are particularly important for large-scale	data management tasks are:

•Scalability
•Cost
•Flexibility
•Availability

### NoSQL types 
	* Column Families: 

Advantages
Most of the solutions, such as Apache Cassandra, HBase, and Google Datastore, allow adding columns over time without having to worry about filling in default values for the existing rows for the new columns. This gives flexibility in model and entity design allowing one to account for new columns in future for unforeseen scenarios and new requirements.

There are advantages when working with a subset of the available columns. For example, computing maxima, minima, averages and sums, specifically on large datasets, is where these column-oriented data stores outshine in performance. Similarly, when new values are applied for either all rows at once or with same-column filters, these databases will allow partial data access without touching unrelated columns and be much faster in execution.

	* Document Store

A document store allows the inserting, retrieving, and manipulating of semi-structured data. Most of the  databases available under this category use XML, JSON, with data access typically over HTTP protocol using RESTful API

Document-oriented databases provide this flexibility—dynamic or changeable schema or even schemaless documents. Because of the limitless flexibility provided in this model, this is one of the more popular models implemented and used. Some of popular databases that provide document-oriented storage include:
• MongoDB
• CouchDB
• Jackrabbit
• Lotus Notes
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
projections
. Each top-level key 
for the JSON object may be the entity's projection across other parts of the system 
thereby allowing the schema to evolve over time with backward compatibilit

	* Key Value

	* Graph Databases

	* Multimodel Databases

## NoSQL Tecnologies

###  Cassandra: Apache Cassandra is open source, distributed data storage system that differs sharply from relational database management systems.

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



##### Advantages

	* 

##### CAP Therorem
	* Consistency
	* Availability
	* Partition Tolerance


### MongoDB
### ElasticSerch
### Elisandra = Elasticserch + Casandra



### OrigenDB 

 
