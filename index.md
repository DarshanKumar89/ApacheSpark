## Putting a Spark in App - Apache Spark

Apache Spark is a fast, in-memory data processing engine with elegant and expressive development APIs to allow data workers to efficiently execute streaming, machine learning or SQL workloads that require fast iterative access to datasets. 
With Spark running on Apache Hadoop YARN, developers everywhere can now create applications to exploit Spark’s power, derive insights
The Hadoop YARN-based architecture provides the foundation that enables Spark and other applications to share a common cluster and dataset while ensuring consistent levels of service and response. Spark is now one of many data access engines that work with YARN in HDP.

- Spark is designed for data science and its abstraction makes data science easier. 
- Data scientists commonly use machine learning – a set of techniques and algorithms that can learn from data. 
- These algorithms are often iterative, and Spark’s ability to cache the dataset in memory greatly speeds up such iterative data processing, making Spark an ideal processing engine for implementing such algorithms.

### Spark Features

Spark takes MapReduce to the next level with less expensive shuffles in the data processing. With capabilities like in-memory data storage and near real-time processing, the performance can be several times faster than other big data technologies.
Spark holds intermediate results in memory rather than writing them to disk which is very useful especially when you need to work on the same dataset multiple times. It’s designed to be an execution engine that works both in-memory and on-disk. Spark operators perform external operations when data does not fit in memory. Spark can be used for processing datasets that larger than the aggregate memory in a cluster.
Spark will attempt to store as much as data in memory and then will spill to disk. It can store part of a data set in memory and the remaining data on the disk. 

### Spark Ecosystem 

ther than Spark Core API, there are additional libraries that are part of the Spark ecosystem and provide additional capabilities in Big Data analytics and Machine Learning areas.
These libraries include:
-Spark Streaming:
Spark Streaming can be used for processing the real-time streaming data. This is based on micro batch style of computing and processing. It uses the DStream which is basically a series of RDDs, to process the real-time data.

-Spark SQL:
Spark SQL provides the capability to expose the Spark datasets over JDBC API and allow running the SQL like queries on Spark data using traditional BI and visualization tools. Spark SQL allows the users to ETL their data from different formats it’s currently in (like JSON, Parquet, a Database), transform it, and expose it for ad-hoc querying.

-Spark MLlib:
MLlib is Spark’s scalable machine learning library consisting of common learning algorithms and utilities, including classification, regression, clustering, collaborative filtering, dimensionality reduction, as well as underlying optimization primitives.

-Spark GraphX:
GraphX is the new (alpha) Spark API for graphs and graph-parallel computation. At a high level, GraphX extends the Spark RDD by introducing the Resilient Distributed Property Graph: a directed multi-graph with properties attached to each vertex and edge. To support graph computation, 

### Apache Spark Use Cases

-Spark Streaming has the capability to handle this extra workload. Some experts even theorize that Spark could become the go-to platform for stream-computing applications, no matter the type
-Streaming ETL – Traditional ETL (extract, transform, load) tools used for batch processing in data.  With Streaming ETL, data is continually cleaned and aggregated before it is pushed into data stores.
-Data enrichment – This Spark Streaming capability enriches live data by combining it with static data, thus allowing organizations to conduct more complete real-time data analysis.
-Trigger event detection – Spark Streaming allows organizations to detect and respond quickly to rare or unusual behaviors (“trigger events”) that could indicate a potentially serious problem within the system. Financial institutions use triggers to detect fraudulent transactions and stop fraud in its tracks. Hospitals also use triggers to detect potentially dangerous health changes while monitoring patient vital signs—sending automatic alerts to the right caregivers who can then take immediate and appropriate action.

-Machine Learning- Spark comes with an integrated framework for performing advanced analytics that helps users run repeated queries on sets of data—which essentially amounts to processing machine learning algorithms. Among the components found in this framework is Spark’s scalable Machine Learning Library (MLlib). The MLlib can work in areas such as clustering, classification, and dimensionality reduction, among many others
-Interactive Analysis   Among Spark’s most notable features is its capability for interactive analytics. MapReduce was built to handle batch processing, and SQL-on-Hadoop engines such as Hive or Pig are frequently too slow for interactive analysis.
-Fog Computing While big data analytics may be getting a lot of attention, the concept that really sparks the tech community’s imagination is the Internet of Things (IoT). The IoT embeds objects and devices with tiny sensors that communicate with each other and the user, creating a fully interconnected world. This world collects massive amounts of data, processes it, and delivers revolutionary new features and applications for people to use in their everyday lives

### Spark In real world
**Netflix** are leveraging Spark for insights and competitive advantage. Other notable businesses also benefitting from Spark are:
**Uber** : Every day this multinational online taxi dispatch company gathers terabytes of event data from its mobile users. By using Kafka, Spark Streaming, and HDFS, to build a continuous ETL pipeline, Uber can convert raw unstructured event data into structured data as it is collected, and then use it for further and more complex analytics.
**Pinterest** – Through a similar ETL pipeline, Pinterest can leverage Spark Streaming to gain immediate insight into how users all over the world are engaging with Pins—in real time. As a result, Pinterest can make more relevant recommendations as people navigate the site and see related Pins to help them select recipes, determine which products to buy, or plan trips to various destinations.
**Conviva** – Averaging about 4 million video feeds per month, this streaming video company is second only to YouTube. Conviva uses Spark to reduce customer churn by optimizing video streams and managing live video traffic—thus maintaining a consistently smooth, high quality viewing experience.

