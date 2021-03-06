# stock-market-microservices
Stock market microservices

# Build
mvn clean package

# Run
docker-compose --compatibility up

# Services links

| Service                | Link                                        | Comments             |
|------------------------|---------------------------------------------|----------------------|
| ActiveMQ               | http://localhost:8161/admin                 | Console              |
| MongoDB                | http://localhost:27017                      | Driver port          |
| Prometheus             | http://localhost:9090                       |                      |
| Grafana                | http://localhost:3000                       | Administration       |
| Elastic search         | http://localhost:9200                       | JSON                 |
|                        | http://localhost:9200/_cat/indices?v&pretty | Elastic indices      |
| Logstash               | http://localhost:9600                       | JSON                 |
| Kibana                 | http://localhost:5601/app/kibana            |                      |
| Config service         | http://localhost:8888                       |                      |
| Discovery service      | http://localhost:8761                       | Eureka               |
| Stock prices producer  | http://localhost:9081/actuator              | Google Metrics       |
|                        | http://localhost:9081/swagger-ui.html       | Google API doc UI    |
|                        | http://localhost:9081/v2/api-docs           | Google API doc json  |
| Stock prices producer  | http://localhost:9082/actuator              | Apple Metrics        |
|                        | http://localhost:9082/swagger-ui.html       | Apple API doc UI     |
|                        | http://localhost:9082/v2/api-docs           | Apple API doc json   |
| Stock prices consumer  | http://localhost:9083/actuator              | Metrics              |
|                        | http://localhost:9083/swagger-ui.html       | API doc UI           |
|                        | http://localhost:9083/v2/api-docs           | API doc json         |
| Zipkin                 | http://localhost:9411                       | Administration       |
