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

