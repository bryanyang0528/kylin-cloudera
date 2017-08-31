# kylin-cloudera
Kylin on cloudera

# Version
Kylin 2.1.0
Cloudera 5.7.0

# Usage
## Run Kylin as a service

1. `sudo docker run --hostname=quickstart.cloudera --privileged=true -t -d  -p 7070:7070 kylin-cloudera:latest`
2. Login to Kylin through `http://<host ip>:7070`   PW:`ADMIN//KYLIN`

## Login to the container
`sudo docker exec -it <container id> /bin/bash`

