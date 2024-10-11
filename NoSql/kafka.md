# Part
- [[Kafka] 프로듀서의 내부 구조와 최적화 전략](https://jinseong-dev.tistory.com/46)

# Kafka Connector
- [Debezium MySQL CDC Source Connector (1)](https://velog.io/@dm911/Debezium-MySQL-CDC-Source-Connector)
- [Debezium으로 DB 동기화 구축하기](https://techblog.uplus.co.kr/debezium%EC%9C%BC%EB%A1%9C-db-synchronization-%EA%B5%AC%EC%B6%95%ED%95%98%EA%B8%B0-1b6fba73010f)
```
connector.class=io.debezium.connector.mysql.MySqlConnector
snapshot.locking.mode=none
database.user=nbtms
database.server.id=100001
tasks.max=1
schema.history.internal.kafka.bootstrap.servers=kafka-flight-log.flight-dev.svc.cd1.io.navercorp.com:9092
snapshot.max.threads=1
database.port=13306
value.converter.schema.registry.url=http://dev.schema.navercorp.com:8081
topic.prefix=mysql
schema.history.internal.kafka.topic=schema-changes.mysql.nbtmsdb
database.hostname=10.168.241.130
database.connectionTimeZone=Asia/Seoul
database.password=nbtms12#$
table.include.list=nbtmsdb.business_travel_invitation
value.converter=io.confluent.connect.avro.AvroConverter
snapshot.mode=initial
```
