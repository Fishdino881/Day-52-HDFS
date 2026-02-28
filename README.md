# Day-52-HDFS

###  Overview

HDFS is the **storage layer of Hadoop**, designed to store **very large files** across multiple machines in a distributed and fault-tolerant way.

It is optimized for **high-throughput data access**, not low latency.

---

##  Key Concepts of HDFS

###  Blocks

* Files are split into large blocks (default: 128 MB)
* Blocks are distributed across the cluster

###  Replication

* Each block is replicated (default: 3 copies)
* Ensures fault tolerance if a node fails

###  NameNode & DataNode

* **NameNode**: Manages metadata (file names, locations)
* **DataNode**: Stores actual data blocks

---

##  Common HDFS Commands

```bash
hdfs dfs -ls /
hdfs dfs -put local.txt /user/data/
hdfs dfs -get /user/data/file.txt
hdfs dfs -rm /user/data/file.txt
hdfs dfs -df -h
```

---

##  Advantages of HDFS

* Handles massive datasets
* Fault tolerant
* Scalable & reliable
* Cost-effective storage
