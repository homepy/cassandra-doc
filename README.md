# cassandra-doc
Cassandra文档输出

## About Apache Cassandra
https://docs.datastax.com/en/cassandra/3.0/index.html

### Overview of Apache Cassandra

Apache Cassandra™ is a massively scalable open source NoSQL database. 
Cassandra is perfect for managing large amounts of structured, semi-structured, and unstructured data across multiple datacenters and the cloud. 
Cassandra delivers continuous availability, linear scalability, and operational simplicity across many commodity servers with no single point of failure, along with a powerful dynamic data model designed for maximum flexibility and fast response times.

### Apache Cassandra 概述

Apache Cassandra™是一个大规模可扩展的开源NoSQL数据库。
Cassandra非常适合在云、多数据中心存储结构化、半结构化、非结构化的数据。
Cassandra在很多商业服务器之间递送了持续可用性，线性扩展，和操作简易性，没有单点故障，同时，它有一个专为高度灵活性和最快的响应时间而设计的，强大的动态的数据模型。


### How does Cassandra work? 

Cassandra’s built-for-scale architecture means that it is capable of handling petabytes of information and thousands of concurrent users/operations per second.

**Cassandra is a partitioned row store database**

Cassandra's architecture allows any authorized user to connect to any node in any datacenter and access data using the CQL language. For ease of use, CQL uses a similar syntax to SQL. The most basic way to interact with Cassandra is using the CQL shell, cqlsh. Using cqlsh, you can create keyspaces and tables, insert and query tables, plus much more. This Cassandra release works with CQL for Cassandra 2.2 and later. If you prefer a graphical tool, you can use DataStax DevCenter. For production, DataStax supplies a number drivers so that CQL statements can be passed from client to cluster and back.

**Automatic data distribution**

Cassandra provides automatic data distribution across all nodes that participate in a ring or database cluster. There is nothing programmatic that a developer or administrator needs to do or code to distribute data across a cluster because data is transparently partitioned across all nodes in a cluster.

**Built-in and customizable replication**

Cassandra also provides built-in and customizable replication, which stores redundant copies of data across nodes that participate in a Cassandra ring. This means that if any node in a cluster goes down, one or more copies of that node’s data is available on other machines in the cluster. Replication can be configured to work across one datacenter, many datacenters, and multiple cloud availability zones.

**Cassandra supplies linear scalability**

Cassandra supplies linear scalability, meaning that capacity may be easily added simply by adding new nodes online. For example, if 2 nodes can handle 100,000 transactions per second, 4 nodes will support 200,000 transactions/sec and 8 nodes will tackle 400,000 transactions/sec:


### Cassandra如何工作？
Cassandra的一切为了可扩展的架构意味着，它能够胜任管理PB级别的数据和每秒上千的并发用户/事务的操作。

**Cassandra是一个分区的行存储数据库**

Cassandra的架构允许任何授权的用户使用CQL语言连接数据中心的任何节点来登陆数据库。为了易用性，CQL使用了跟SQL相似的语法规则。和Cassandra交互的最基本的方法是使用CQL shell ，cqlsh命令。使用cqlsh，你可以创建keyspaces和tables，向table里插入和查询以及更多操作。这个Cassandra的发行版适用于Cassandra 2.2的CQL和后来的版本。如果你想使用图形界面工具，你可以使用DataStax DevCenter.
为了生产使用，DataStax提供了一系列的驱动，使CQL表达式可以从客户端传输到集群然后返回。

**数据自动分区**

Cassandra提供了在所有节点之间的数据自动分区方法，然后数据加入到一个环或者数据集群里。开发者或者管理员不需要写代码来把数据分布到集群中去，因为数据是透明分区在集群的所有节点中的。

**内置的和可定制的复制策略**

Cassandra也提供了内置的和可定制的复制策略，在多个节点上保存着冗余的备份，并且加入到Cassandra环中。这意味着如果集群中的任何节点挂掉，在集群中的其他机器上还有一份或者多份节点的可用数据备份。备份策略可以配置成一个数据中心，多个数据中心，和多个云可用区域。

**Cassandra可线性扩展**

Cassandra提供了线性可扩展，意味着存储空间可以简单的通过在线添加新节点来增加容量。举个例子，如果2个节点可以处理每秒100,000个事务，那么4个节点可以支持每秒200,000个事务，8个节点可以解决每秒400,000个事务。
