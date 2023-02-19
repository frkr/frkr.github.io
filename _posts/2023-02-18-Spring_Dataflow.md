---
title: SpringDataflow
layout: post
post-image: https://i.ytimg.com/vi/rvAr0KYXBhk/maxresdefault.jpg
tags:
- Spring
- SpringDataflow
- SpringCloud
- SpringCloudDataflow
- Workflow
- Pipeline
---

# Spring Dataflow


## Instalação Local, vem vazia
- [Testar com Kubernetes](https://docs.spring.io/spring-cloud-dataflow/docs/current/reference/htmlsingle/#local-k8s-development)


### Arquivos
- [DOC](https://dataflow.spring.io/docs/installation/local/docker/) / [PDF](/assets/springdataflow/local-spring-dataflow.pdf)
- [YAML Compose](/assets/springdataflow/docker-compose.yml)
- [YAML RabbitMQ](/assets/springdataflow/docker-compose-rabbitmq.yml)
- [YAML MySQL](/assets/springdataflow/docker-compose-mysql.yml)

```shell

wget -O docker-compose.yml https://raw.githubusercontent.com/spring-cloud/spring-cloud-dataflow/main/src/docker-compose/docker-compose.yml;
wget -O docker-compose-rabbitmq.yml https://raw.githubusercontent.com/spring-cloud/spring-cloud-dataflow/main/src/docker-compose/docker-compose-rabbitmq.yml;
wget -O docker-compose-mysql.yml https://raw.githubusercontent.com/spring-cloud/spring-cloud-dataflow/main/src/docker-compose/docker-compose-mysql.yml;

export DATAFLOW_VERSION=2.10.1
export SKIPPER_VERSION=2.9.1
docker-compose -f docker-compose.yml -f docker-compose-rabbitmq.yml -f docker-compose-mysql.yml up

```

- http://localhost:9393/dashboard
- http://localhost:7577/api
