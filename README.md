# proxeneta
The proxeneta project. Demo

```mermaid
flowchart TD;
    subgraph Producer
        direction LR
    Kafka
    Consumer
    Producer --> Kafka
    Kafka --> Consumer
```
