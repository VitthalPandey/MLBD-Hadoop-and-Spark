 **Overview**

This assignment focuses on practical implementation and analysis of big data processing frameworks, specifically Apache Hadoop and Apache Spark. The tasks include setting up a local Hadoop environment, executing MapReduce programs, working with HDFS, and performing large-scale text analytics using PySpark.

The project demonstrates how distributed systems handle large datasets efficiently through parallel computation, fault tolerance, and scalable storage.

  **Objectives**

Install and configure Hadoop on Ubuntu

Understand HDFS architecture and operations

Execute MapReduce WordCount program

Analyze performance parameters

Extract metadata from large text collections

Compute document similarity using TF-IDF

Construct an author influence network

Gain hands-on experience with PySpark

 **System Configuration**

Operating System: Ubuntu 22.04

Hadoop Version: 3.3.x

Java Version: OpenJDK 8/11

Spark Version: 3.x

Python Version: 3.x

Mode: Pseudo-Distributed

  **Hadoop Installation**

Hadoop was installed and configured following the guide:

🔗 https://medium.com/@abhikdey06/apache-hadoop-3-3-6-installation-on-ubuntu-22-04-14516bceec85

Configuration included:

Setting environment variables

Configuring core-site.xml, hdfs-site.xml, mapred-site.xml, yarn-site.xml

Formatting HDFS NameNode

Starting HDFS and YARN services

  **Hadoop Tasks (Q1–Q9)**
✔ WordCount MapReduce Program

Implemented using Hadoop examples

Demonstrates distributed processing

Output shows word frequencies

✔ HDFS Operations

Uploading and managing files

Block storage and replication

Directory management

✔ Performance Analysis

Execution time measured using system timestamps

Effect of input split size evaluated

  **Spark Tasks (Q10–Q12)**
✔ Metadata Extraction

Metadata fields (title, release date, language, encoding) were extracted from Project Gutenberg texts using regular expressions.

✔ Document Similarity (TF-IDF)

Steps performed:

Text preprocessing

Tokenization

Stop-word removal

TF computation

IDF computation

TF-IDF vector generation

Cosine similarity calculation

This identifies books similar to a target text.

✔ Author Influence Network

An influence network was constructed based on publication years to approximate relationships between authors.

**Key Concepts Used**

Distributed Storage (HDFS)

MapReduce Programming Model

Parallel Processing

Regular Expressions for Text Parsing

TF-IDF Vectorization

Cosine Similarity

Graph Representation of Relationships

Spark DataFrames and SQL Operations

******Results**

Hadoop successfully processed large text data using MapReduce.

Performance depended on input split size and cluster configuration.

Spark efficiently handled metadata extraction and similarity analysis.

TF-IDF effectively highlighted meaningful terms.

Influence network provided insights into relationships between authors.

**Limitations**

Influence relationships are approximated using publication year only.

Metadata inconsistencies may affect extraction accuracy.

Cross-join operations scale poorly for very large datasets.
