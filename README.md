# ELK_docker_logaggregator
This repos contains two folder
1. Server
2. Client

Server:
It has docker stack file which can be deployed as docker service in docker swarm cluster
Docker stack contains:
a. Elastisearch
b. Logstash
c. Kibana
It also contains logstash conf file which is used by the docker stack file to provide the configuration for logstash component.

Clients:
The client is the one which sends the data to the ELK server and the data can be viewed in kibana.
These clients are called as Beats. There are many pre-built beats are there. We can even develop our own builds.
e.g. to pre-built beats
a. Filebeat(monitor the files)
b. WinLogBeat(monitor the windows event)
c. MetricBeat(Monitor the windows machine health)
Currently this folder contains the filebeat.yml which will listen to iis logs and send to logstash.
