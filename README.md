# Docker-Elastic-Beats

load filebeat-dashboards
````
docker run --net="host" docker.elastic.co/beats/filebeat:7.16.0 setup --dashboards
````

load metricbeat-dashboards
````
docker run --net="host" docker.elastic.co/beats/metricbeat:7.16.0 setup --dashboards
````

load packetbeat-dashboards
````
docker run --cap-add=NET_ADMIN --net="host" docker.elastic.co/beats/packetbeat:7.16.0 setup --dashboards
````