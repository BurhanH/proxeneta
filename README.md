# proxeneta
The proxeneta project. Demo

```mermaid
flowchart TD;
    subgraph Producer;
        direction TB;
        database1;
        cache1;
        service1;
        API1;
    end
    subgraph Kafka;
        direction TB;
        nodes;
        topics;
        partitions;
    end
    subgraph Consumer;
        direction TB;
        database2;
        cache2;
        service2;
        API2;
    end

    Producer --> Kafka;
    Kafka --> Consumer;
```
