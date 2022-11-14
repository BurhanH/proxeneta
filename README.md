# proxeneta
The proxeneta project. Demo

```mermaid
flowchart TD;
    subgraph Producer;
        direction LR;
        database;
        cache;
        service;
        API;
    end
    subgraph Kafka;
        direction TB;
        nodes;
        topics;
        partitions;
    end
    subgraph Consumer;
        direction LR;
        database;
        cache;
        service;
        API;
    end
    Producer --> Kafka
    Kafka --> Consumer
```
