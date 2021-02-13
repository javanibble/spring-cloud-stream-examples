

## Sample Data

```json
{"name": "Tony Stark", "age": 34,"gender": "male"}

{"name": "Black Panther", "age": 34,"gender": "male"}

```

## Commands
```bash
# Start Kafka
$ confluent local services start

# Browser: http://localhost:9021/
# Create Topic: test-topic

$ kafka-topics --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic my-topic

$ kafka-console-producer --topic my-topic --bootstrap-server localhost:9092
$ kafka-console-consumer --topic my-topic --bootstrap-server localhost:9092 --from-beginning

$ confluent local services stop
$ confluent local destroy
```
