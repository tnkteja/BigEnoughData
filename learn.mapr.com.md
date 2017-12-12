## Introduction to Big data : Summary

High Volume , Variety, Velocity

### High Volumne
As of 2014 Nasa Generated 1.73 GB/s .

### High Variety
wikipedia, contains all kinds of data, text, links, media,
types
```python
class DataVarietyType(object):
    def __init__(self):
        pass
        
class Structured(DataVarietyType):
    pass
    
class SemiStructured(DataVarietyType):
    """
    emails
    """
    pass

class Unstructured(DataVarietyType):
    """
    video files
    """
    pass


```
### High Velocity

Example: google internet catalogging problem

High Volume - catalogging whole internet.
High Velocity- updates made to webpages at high velocity.
* Traditional databases cannot handle the speed of updates. as a result of updates made by the webpages every day.
High Variety - web pages contain all types of data.

Answer - MapReduce, Bigtable, GFS

* Google File System - splitting into chunks replicated across nodes
* Bigtable
    * uses timestamp to avoid overides
    * tablets - parts of the rows.
    
 Mapreduce - comes all the way  `LISP`
 using mapreduce - comes from 19th se to one.
 page rank algorithm
 ```python
 # Python Analogous
 
 kvs={}
 keys=kvs.keys()
 contents=kvs.contents()
 map(lambda k,c:  for word in c:  (word,'1'),keys,contents)
 
 
 ```
 
 using published papers from google - Doug Cutting developed Opensource Apache Hadoop, hadoop begin his sons toy elephant.
 
Google|Hadoop|Mapr
:-:|:-:|:-:
MapReduce|MapReduce| MapReduce
Bigtable|HBase|HBase/MapR-DB
GFS|HDFS|HDFS/MapR-FS

Commercial
1000 MB = 1 GB 
1000 GB = 1 TB
1000 TB = 1 PB

Types of data -  computer science data types
* chartacter
* string
* integer
* float

other
* timestamps
* date
* images
* sounds
* videos

types of files
```python
class SimpleStructed():
    """
    spreadsheet as csv file
    """
    pass
class ComplexStructured():
    """
    Parquet
    """
    pass
class SimpleSemi-Structured():
    """
    Apache HBase
    """
    pass
    
class ComplexSemiStructured():
    """
    Json
    """
    pass

    
```

Physical  Storage | Logical Storage
:-:|:-:
Actual real world location of your data | how OS organizes the data

Common Terms - 
* ETL ( Extract Transform Load )
* IoT ( Internet of Things )
* SQL ( Sequentiall Query Language )
* JSON ( Javascript Object Notation)
* API ( Application Programming Interface )
* UDF ( User defined functions ) - had to search this one :( - frowny face )

```Python

class DataSource(object):
    pass
    
class DataIngestion(object):
    pass
    
class DataProcessing(object):
    pass

class DataAnalysis(object):
    pass
    
```

* Define your project
* Data architect can map out data pipeline

Common Questions
How and Why are you collecing data ? ( Not quite the question for what wanted to start for )
Velocity - How ( questionalble)
    * Streaming => real time
    * Batch => no immediete acction
       * historical records
Variety - what kind ( fine )
Volumne - how much
usually 4 x data
 3 replicas + space for OS + space for meta data files
 
Extract => Transform ( Normalizing, Cleaning, Sampling, Splitting ) => Load

Final Step data analysis
