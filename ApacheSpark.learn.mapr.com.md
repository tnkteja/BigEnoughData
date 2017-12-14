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
