---
title: SpringDataflow
layout: post
post-image: https://dataflow.spring.io/static/21b104023960490a68239f328ac8055e/ee604/screen-dataflow.png
---

### DataFlow
- [DOC](https://dataflow.spring.io/docs/installation/local/docker/)
- [PDF](/assets/springdataflow/spring-data-flow-reference.pdf)

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
