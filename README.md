# Energy Platform Architecture

Repository for system architecture, diagrams, and technical decisions  
for the energy trading platform (solar power plants, real-time telemetry, and trading).


## Structure
```text
/c1 - System Context diagrams (high-level view)
/c2 - Container diagrams (services, Kafka, Edge, etc.)
/c3 - Component diagrams (internal structure of services)
/events - Event definitions (Kafka topics, payloads)
/api - API contracts (HTTP, external integrations)
/adr - Architecture Decision Records
```

## Diagrams
All diagrams are created using Eraser and follow the C4 model:

- C1 – System Context
- C2 – Containers (main system architecture)
- C3 – Components (service internals)

For online visualization of circuits use - https://app.eraser.io/

## Event Flow
- Telemetry flows from solar plants → central platform
- Events are processed asynchronously via Kafka
- Trading decisions generate commands back to plants


## Documentation Rules
- Any architecture change → update diagrams
- Any major decision → create ADR
- Events  must be documented
