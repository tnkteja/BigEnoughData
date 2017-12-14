* Cluster computing platform on top of storage layer
* Extends mapReduce with support for 
    * Streaming
    * Interactive analytics
* Runs in memory by default 100x faster than mapReduce

10x faster than mapreduce, on disk

* Write programs quickly
* More operators
* Interactive Shell
* Less code

Deployment options
* Mesos
* YARN
* Standalone
* Local
```python
class Deployment(object):
    def __init__(self):
        pass
class Mesos(Deployment):
    def __init__(self):
        pass
class YRN(Deployment):
    def __init__(self):
        pass
        
class Standalone(Deployment):
     def __init__(self):
         pass

class Local(Deployment):
    def __init__(self):
        pass
        
```
Storage options
* MapR-FS
* HDFS
* S3
```python
class Storage(object):
    def __init__(self):
        pass
        
class MapRFS(object):
    def __init__(self):
        pass
class HDFS(object):
    def __init__(self):
        pass
class S3(object):
    def __init__(self):
        pass
```
Stack
* Batch/ETL  Processing: Spark, MapReduce, Hive, Pig
* Stream Processing: Spark Streaming, Storm
* Machine Learning: Spark MLlib, Mahout
* Quieries: Spark SQL, Drill, Hive
* Graphprocessing: Sprak GraphX, Giraph, Graphlab

Spark on MAPR/HADOOP

Use cases
* OLAP Analytics
* Operational Analytics
* Complex data Pipeliining
```python
class UseCase(object):
    pass
    
class OLAPAnalytics(object):
"""
Service provider using MapR and Spark delivers real-time multi-dimensional OLAP analytics 
Must accept data of any type/format
Perform rigorous analytics across large datasets
"""
    def __init__(self):
        pass

class operationalAnalytics(UseCase):
"""
Health Insurance company uses MapR to store patient information
Spark computes patient re-admittance probability
Real-time analytics over NoSQL
Spark with MapR-DB
"""
    def __init__(self):
        pass
class  ComplexDataPipelining(UseCase):
"""
Pharmaceutical company uses Spark on MapR for gene sequencing analysis
Spark reduces processing from weeks to hours
Complex machine learning without MapReduce
"""
    def __init__(self):
        pass
```

```python
class RDD(object):
    pass
    def transform(self):
       pass
```
![libraries](http://1cf3dc78d0105c23703f-c41db0b1ded8e000fd0c1ba57f8ba402.r14.cf1.rackcdn.com/global/imagelib/edu_ess360/ess320_sparklibraries.png)
