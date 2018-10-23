# ansible-redis-cluster
The role is currently broken into 3 parts:
 - redis/core : to install the required components for redis
 - redis/node : which will configure everything for a node, and get it running
 - redis/cluster : Use to create the cluster from the individual nodes
 
 make sure there is no redis process in each node server, otherwise cluster will fail
 ps -ef | grep redis | awk '{print $2}' | xargs kill -9