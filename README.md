# kylin-cloudera

[Kylin](http://kylin.apache.org/) is an open source Distributed Analytics Engine designed to provide SQL interface and multi-dimensional analysis (OLAP) on Hadoop supporting extremely large datasets, original contributed from eBay Inc.

This docker images which Kylin is installed is based on Cloudera.
User can choose Spark as the computing engine in this image.

**Any feedback is welcome**

# Version

* Kylin 2.1.0
* Cloudera 5.7.0
* Hadoop 2.6.0-cdh5.7.0
* HBase 1.2.0-cdh5.7.0
* Spark 1.6.0
* Hive 1.1.0

# Usage
## Run Kylin as a service

1. `sudo docker run --hostname=quickstart.cloudera --privileged=true -t -d  -p 7070:7070 kylin-cloudera:latest`
2. Login to Kylin through `http://<host ip>:7070`   PW:`ADMIN//KYLIN`

## Login to the container
`sudo docker exec -it <container id> /bin/bash`

