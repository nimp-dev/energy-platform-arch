# ADR-001: Use Kafka as Event Backbone

## Status
Develop

## Context
The system requires real-time processing of telemetry data from multiple solar plants,
high throughput, and the ability to replay events.

## Decision
We use Apache Kafka as the central event streaming platform.

## Alternatives
- RabbitMQ – rejected due to lower throughput and limited replay capabilities
- REST-based communication – rejected due to tight coupling

## Consequences

## Positive
- High scalability
- Event replay support
- Decoupled services

### Negative
- Increased complexity
- Requires operational expertise