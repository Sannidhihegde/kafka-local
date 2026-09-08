# kafka-local

Local infrastructure for running this project's services during
development: a Kafka broker (KRaft mode, no Zookeeper) and a Zipkin
instance. Purely a local dev convenience — not deployed anywhere.

## Usage
    docker compose up -d

- Kafka broker: `localhost:9092`
- Zipkin UI: `http://localhost:9411`

## Used by
- Kafka: [inventory-service](https://github.com/Sannidhihegde/inventory-service) (producer), [agent-service](https://github.com/Sannidhihegde/agent-service) (producer), [audit-service](https://github.com/Sannidhihegde/audit-service) (consumer), [notification-service](https://github.com/Sannidhihegde/notification-service) (consumer)
- Zipkin: intended for all request-path services (tracing currently parked —
  see agent-service's README status notes for known Boot 4.1.x upstream
  issues)
