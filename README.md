# ansible-redis-cluster
The role is currently broken into 3 parts:
 - redis/core : to install the required components for redis
 - redis/node : which will configure everything for a node, and get it running
 - redis/cluster : Use to create the cluster from the individual nodes