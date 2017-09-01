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
## Pull images

[Kylin-Cloudera](https://hub.docker.com/r/bryanyang0528/kylin-cloudera/)

`docker pull docker pull bryanyang0528/kylin-cloudera`

## Build the Dockerfile (Optional)

1. `git clone https://github.com/bryanyang0528/kylin-cloudera`
2. `cd kylin-cloudera`
3. `sudo docker build -t kylin-cloudera:latest .`

## Run Kylin as a service

1. `sudo docker run --hostname=quickstart.cloudera --privileged=true -t -d  -p 7070:7070 kylin-cloudera:latest`
2. Login to Kylin through `http://<host ip>:7070/kylin/login`   PW:`ADMIN//KYLIN`

## Login to the container
`sudo docker exec -it <container id> /bin/bash`

## Ports of Services

* 80L Cloudera Tutorial
* 7070: Kylin
* 8888: Hue
* 18080: Spark Web UI
* 50070: Hadoop NameNode 
