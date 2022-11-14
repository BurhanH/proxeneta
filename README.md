# proxeneta
The proxeneta project. Demo

```mermaid
flowchart TD;
    subgraph Producer;
        direction TB;
        p-database;
        p-cache;
        p-service;
        p-API;
        p-gRPC;
    end
    subgraph Kafka;
        direction TB;
        nodes;
        topics;
        partitions;
    end
    subgraph Consumer;
        direction TB;
        c-database;
        c-cache;
        c-service;
        c-API;
        c-gRPC;
    end
    subgraph Monitor;
        direction TB;
        m-API;
        m-gRPC;
    end

    Producer --> Monitor;
    Consumer <-- Monitor;
    Producer --> Kafka;
    Kafka --> Consumer;
```
