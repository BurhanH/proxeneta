# proxeneta
The proxeneta project. Demo

```mermaid
flowchart TD;
    Subgraph Producer;
        direction LR;
    Kafka;
    Consumer;
    Producer --> Kafka;
    Kafka --> Consumer;
```
