# Kafka-consumers-starter

### Determine your cluster endpoint
`confluent kafka cluster describe`

### Execute script
`./consumer.py config.ini`

### Consume messages from a topic
`confluent kafka topic consume --from-beginning {TOPIC_NAME}`

### To properly read the data, tell the consumer to fetch the Avro schema from Schema Registry and deserialize the data
`confluent kafka topic consume --value-format avro --schema-registry-api-key {API Key} --schema-registry-api-secret {API Secret} {TOPIC_NAME}`
