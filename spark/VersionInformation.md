Spark Versions and Builds Available 
===================================

For installation and examples see  [README.md](README.md).


Each of the below EMR AMIs will install the last Spark build available for that AMI.


To request a specific Spark version build use "-v" to request a specific build version.   


* Hadoop 1.0.3 (AMI 2.x)
 * Spark 0.8.1

* Hadoop 2.2.0 (AMI 3.0.x)
 * Spark 1.0.0

* Hadoop 2.4.0 (AMI 3.1.x and 3.2.0-3.2.3)
 * Spark 1.0.2
 * Spark 1.1.0
 * Spark 1.1.0.b (built with httpclient 4.2.5 to fix version conflict with AWS SDK)
 * Spark 1.1.0.c (spark-submit deploy mode default changed to cluster, kinesis examples included, ganglia metrics plugin included, sql hive dependencies fixed)
 * Spark 1.1.0.d (kinesis jars added to lib, added JavaKinesisWordCountASLYARN example which uses yarn-cluster for master)
 * Spark 1.1.0.e (kinesis example sources added to examples dir, includes SPARK-3595 for correct S3 output handling)
 * Spark 1.1.0.f (install script change to work with EMR AMI 3.1.4, 3.2.3 and later)
 * Spark 1.1.0.g (disables multipart upload for Hadoop output formats as workaround, Enables Pyspark support)
 * Spark 1.1.0.h (same as "g", rebuilt with git repo)  [NOTE: Last version of 1.1.0 release ]


* Hadoop 2.4.0 (AMI 3.3.x and 3.4.x)
 * Spark 1.1.1.a (Initial version of Spark's 1.1.1 release with select changes for working on EMR)
 * Spark 1.1.1.b (Include SPARK-3595 for EMR S3 output without temporary directory)
 * Spark 1.1.1.c (Change to class path for hadoop-provided profile build, Fix to support hive-site.xml and hive-default.xml with spark-sql)
 * Spark 1.1.1.d (Addition of JVM options for GC, Add Hbase and Kinesis client jars available to classpath)
 * Spark 1.1.1.e (SparkSQL support for EMR S3 output without temporary directory)
 * --
 * Spark 1.2.0.a (Initial build of Spark's 1.2.0 release)
 * Spark 1.2.1.a (Initial build of Spark's 1.2.1 release)

* Hadoop 2.4.0 (AMI 3.5.x)
 * *Spark 1.3.0.a (Initial build of Spark's 1.3.0 release)*

#### Experimental versions available (designed to be ran with latest AMI available at time of build)
* branch-1.1 ( "-v 1.1 -b \<buildId\>")
 * 2014112801 (includes SPARK-2848)
 * 2014121700
* branch-1.2 ( "-v 1.2 -b \<buildId\>")
 * 2014120500
 * 2014121700

