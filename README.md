# kafka-elastic
Monitoring Kafka JMX metrics with beats/elasticsearch/kibana.

## Containers

This docker-compose contains following containers.
- Apache Kafka (base image)
  - [wurstmeister/kafka](https://hub.docker.com/r/wurstmeister/kafka/)

    Build a container by adding [jolokia Java agent](https://jolokia.org/).
- Zookeeper
  - [wurstmeister/zookeeper](https://hub.docker.com/r/wurstmeister/zookeeper/)
- elasticsearch
  - [elasticsearch](https://github.com/elastic/elasticsearch)
- kibana
  - [kibana](https://github.com/elastic/kibana)
- metriceat
  - [metricbeat](https://github.com/elastic/beats)

## Install

`docker-compose up`

## Access to prometheus and grafana

- kibana

  http://localhost:5601
