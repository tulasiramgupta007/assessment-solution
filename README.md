# assessment-solution

first i download the python 3.8 and install and set it up and set the environment path also.
then i download the java and install and set it up and set the environment path also.
then i download the spark version 3.1.3 and hadoop version 2.7 and install and set it up and set the environment path also.
then in command prompt shell i make a directory of spark and hadoop\bin and also set path for hadoop in environment.
then in spark directory i ran this code to install and run spark - spark-3.1.3-bin-hadoop2.7\bin\spark-shell
this code install the spark in my system then in spark directory i write 'pyspark' for pyspark run.
then import the spark session - from pyspark.sql import SparkSession
then create the spark session - 
>>> spark = SparkSession \
...     .builder \
...     .appName("how to read csv file") \
...     .getOrCreate()

then read the csv file  - 
df = spark.read.csv(r'C:\Users\hp\Downloads\Assessment/people.csv',header=True)

Show record count for above dataframe - df.count()

it gives the value of 40 records.
