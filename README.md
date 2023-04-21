
# Big Data Analytics for Airlines Traffic using Java MapReduce and Hive

This repository contains a Java MapReduce program and Hive queries for analyzing airline traffic data. The data used in this project is the "On-Time Performance" data from the United States Department of Transportation's Bureau of Transportation Statistics.


## Prerequisites 

To run this program, you will need:

* Hadoop
* Hive
* Java Development Kit (JDK)
## Getting Started

1. Clone the repository using the command:
```bash
git clone https://github.com/nikku0009/AirlinesBigDataAnalytics.git
```

2. Load the data into Hadoop using the following command:
```bash
hadoop fs -put <path_to_data_file> <hdfs_path_to_store_data>
```

3. Build the Java MapReduce program using the following command:
```bash 
javac -classpath <path_to_hadoop_jars> -d <output_directory> AirlinesTraffic.java
```

4. Run the Java MapReduce program using the following command:
```bash 
hadoop jar <path_to_hadoop_jars> -classpath <output_directory> AirlinesTraffic <input_path> <output_path>
```

5. Execute the Hive queries using the following command:

```bash 
hive -f airlines_traffic_analysis.hql
```




## Output

The Java MapReduce program outputs a CSV file containing the analysis of the airline traffic data. The Hive queries output the results of the data analysis in a tabular format.
