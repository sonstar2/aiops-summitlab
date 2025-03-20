# aiops-summitlab
This repo will be used for the Summit 2025 AIOps Lab










## Working with Kafka


Here are some basic commands and troubleshooting:


1. List all topics on kafka:

```bash
podman exec cp-kafka /opt/kafka/bin/kafka-topics.sh --list --bootstrap-server localhost:9092
```

2. Creating a topic called `httpd-error-logs`:

```bash
podman exec cp-kafka /opt/kafka/bin/kafka-topics.sh --create --topic httpd-error-logs --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
```