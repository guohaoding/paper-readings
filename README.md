# Readings in Databases
A list of database-related papers
## Table of Contents
1. [Data loading](#data-loading)
2. [SQL on Hadoop](#sql-on-hadoop)
3. [Batch processing](#batch-processing)
4. [Stream processing](#stream-processing)
5. [Coordination](#coordination)

## <a name="data-loading"> Data loading
 * Tobias Mühlbauer, Wolf Rödiger, Robert Seilbeck, Angelika Reiser, Alfons Kemper, Thomas Neumann. [Instant Loading for Main Memory Databases](http://www.vldb.org/pvldb/vol6/p1702-muehlbauer.pdf), VLDB, 2013
 * K.T. Sridhar and M.A. Sakkeer. [Optimizing Database Load and Extract for Big Data Era](https://link.springer.com/content/pdf/10.1007%2F978-3-319-05813-9_34.pdf), DASFAA, 2014
 * Adam Dziedzic, Manos Karpathiotakis, Ioannis Alagiannis, Raja Appuswamy, Anastasia Ailamaki. [DBMS Data Loading: An Analysis on Modern Hardware](http://www.adms-conf.org/2016/dziedzic_adms16.pdf)([slides](http://www.adms-conf.org/2016/loading-adms-presentation.pdf)), ADMS(VLDB workshop), 2016
### In Situ Data Processing
 * Stratos Idreos, Ioannis Alagiannis, Ryan Johnson, Anastasia Ailamaki. [Here are my Data Files. Here are my Queries. Where are my Results?](http://cidrdb.org/cidr2011/Papers/CIDR11_Paper7.pdf)([slides](http://cidrdb.org/cidr2011/Talks/CIDR11_Papa.pptx)), CIDR, 2011
 * Ioannis Alagiannis, Renata Borovica, Miguel Branco, Stratos Idreos, Anastasia Ailamaki. [NoDB: Efficient Query Execution on Raw Data Files](https://infoscience.epfl.ch/record/213746/files/nodb-cacm.pdf)([slides](http://renata.borovica-gajic.com/data/slides/sigmod2012_nodb.pdf), [poster](http://renata.borovica-gajic.com/data/poster/sigmod2012_nodb.pdf)), SIGMOD, 2012
 * Azza Abouzied, Daniel J. Abadi, Avi Silberschatz. [Invisible Loading: Access-Driven Data Transfer from Raw Files into Database Systems](https://openproceedings.org/2013/conf/edbt/AbouziedAS13.pdf), EDBT/ICDT, 2013
### Parsing
 * Yinan Li, Nikos R. Katsipoulakis, Badrish Chandramouli, Jonathan Goldstein, Donald Kossmann. [Mison: A Fast JSON Parser for Data Analytics](http://www.vldb.org/pvldb/vol10/p1118-li.pdf), PVLDB, 2017
 * Shoumik Palkar, Firas Abuzaid, Peter Bailis, Matei Zaharia. [Filter Before You Parse: Faster Analytics on Raw Data with Sparser](https://www.vldb.org/pvldb/vol11/p1576-palkar.pdf)([slides](https://www.slideshare.net/databricks/sparser-faster-parsing-of-unstructured-data-formats-in-apache-spark-with-firas-abuzaid-and-shoumik-palkar?from_action=save),[DAWN-Sparser](https://dawn.cs.stanford.edu/2018/08/07/sparser/)), PVLDB, 2018

## <a name="sql-on-hadoop"> SQL on Hadoop
 * Ashish Thusoo, Joydeep Sen Sarma, Namit Jain, Zheng Shao, Prasad Chakka, Ning Zhang, Suresh Anthony, Hao Liu, Raghotham Murthy. [Hive - a petabyte scale data warehouse using Hadoop](papers/2010-Hive.pdf)([slides](slides/Hive-Raghotham%20Murthy.pdf)), ICDE, 2010
 * 	Jesús Camacho-Rodríguez, Ashutosh Chauhan, Alan Gates, Eugene Koifman, Owen O'Malley, Vineet Garg, Zoltan Haindrich, Sergey Shelukhin, Prasanth Jayachandran, Siddharth Seth, Deepak Jaiswal, Slim Bouguerra, Nishant Bangarwa, Sankar Hariappan, Anishek Agarwal, Jason Dere, Daniel Dai, Thejas Nair, Nita Dembla, Gopal Vijayaraghavan, Günther Hagleitner. [Apache Hive: From MapReduce to Enterprise-grade Big Data Warehousing](papers/2019-Hive.pdf)
 * Reynold S. Xin, Josh Rosen, Matei Zaharia, Michael J. Franklin, Scott Shenker, Ion Stoica. [Shark: SQL and rich analytics at scale](papers/2013-Shark.pdf), SIGMOD, 2013
 * Michael Armbrust, Reynold S. Xin, Cheng Lian, Yin Huai, Davies Liu, Joseph K. Bradley, Xiangrui Meng, Tomer Kaftan, Michael J. Franklin, Ali Ghodsi, Matei Zaharia. [Spark SQL: Relational Data Processing in Spark](papers/2015-Spark%20SQL.pdf), SIGMOD, 2015

## <a name="batch-processing"> Batch processing
 * Jeffrey Dean and Sanjay Ghemawat. [MapReduce: Simplified Data Processing on Large Clusters](papers/2004-MapReduce.pdf)([slides](slides/MapReduce-Jeff%20Dean.ppt)), OSDI, 2004
 * Matei Zaharia, Mosharaf Chowdhury, Michael J. Franklin, Scott Shenker, Ion Stoica. [Spark: Cluster Computing with Working Sets](papers/2010-Spark.pdf)([slides](slides/Spark-Zaharia.pdf)), HotCloud, 2010
 * Matei Zaharia, Mosharaf Chowdhury, Tathagata Das, Ankur Dave, Justin Ma, Murphy McCauley, Michael J. Franklin, Scott Shenker, Ion Stoica. [Resilient Distributed Datasets: A Fault-Tolerant Abstraction for In-Memory Cluster Computing](papers/2012-RDD.pdf)([slides](slides/RDD-zaharia.pdf)), NSDI, 2012

## <a name="stream-processing"> Stream processing
 * Ankit Toshniwal, Siddarth Taneja, Amit Shukla, Karthik Ramasamy, Jignesh M. Patel*, Sanjeev Kulkarni, Jason Jackson, Krishna Gade, Maosong Fu, Jake Donham, Nikunj Bhagat, Sailesh Mittal, Dmitriy Ryaboy. [Storm @Twitter](papers/2014-Storm.pdf)([slides](slides/Storm-Karthik%20Ramasamy.pdf)), SIGMOD, 2014
 * Matei Zaharia, Tathagata Das, Haoyuan Li, Scott Shenker, Ion Stoica. [Discretized Streams: An Efficient and Fault-Tolerant Model for
Stream Processing on Large Clusters](papers/2012-Spark%20Streaming.pdf)([slides](slides/Spark%20Streaming-Zaharia.pdf)), HotCloud, 2012
 * Matei Zaharia, Tathagata Das, Haoyuan Li, Timothy Hunter, Scott Shenker, Ion Stoica. [Discretized Streams: Fault-Tolerant Streaming Computation at Scale](papers/2013-Spark%20Streaming.pdf)([slides](slides/Spark%20Streaming-Tathagata%20Das(SOSP).pptx)), SOSP, 2013
 * Paris Carbone, Asterios Katsifodimos, Stephan Ewen, Volker Markl, Seif Haridi, Kostas Tzoumas. [Apache Flink: Stream and Batch Processing in a Single Engine](papers/2015-Flink.pdf)([slides](slides/Flink-Paris%20Carbone.pdf)), 2015

## <a name="coordination"> Coordination
 * Mike Burrows. [The Chubby lock service for loosely-coupled distributed systems](papers/2006-Chubby.pdf), OSDI, 2006
 * Patrick Hunt, Mahadev Konar, Flavio Paiva Junqueira, Benjamin Reed. [ZooKeeper: Wait-free coordination for Internet-scale systems](papers/2010-Zookeeper.pdf)([slides](slides/Zookeeper-Benjamin%20Reed.pdf)), USENIX ATC, 2010
