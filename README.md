# kafka-local

Local Kafka broker (KRaft mode, no Zookeeper) for running this project's services
during development. Purely a local dev convenience — not deployed anywhere.

## Usage
    docker compose up -d
Broker available at `localhost:9092`.

## Used by
[inventory-service](https://github.com/Sannidhihegde/inventory-service) (producer),
[agent-service](https://github.com/Sannidhihegde/agent-service) (producer),
[audit-service](https://github.com/Sannidhihegde/audit-service) (consumer),
[notification-service](https://github.com/Sannidhihegde/notification-service) (consumer)
