
# List all kafka topics
./bin/kafka-topics.sh --list --zookeeper "zookeeper:2181"

# Schema change watch event
./bin/kafka-console-consumer.sh --bootstrap-server "kafka:9092" --topic "schema-changes.inventory" --from-beginning

# Watch change event
./bin/kafka-console-consumer.sh --bootstrap-server "kafka:9092" --topic "dbserver_1.inventory.customers" --from-beginning

