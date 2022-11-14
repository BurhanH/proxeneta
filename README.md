# proxeneta
The proxeneta project. Demo

```mermaid
flowchart TD;
    subgraph Producer
        direction LR
        database
        cache
        service
        API

    subgraph Kafka
        direction TB
        nodes
        topics
        partitions

    subgraph Consumer
        direction LR
        database
        cache
        service
        API

    Producer --> Kafka
    Kafka --> Consumer
```
