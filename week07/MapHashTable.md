## Map/Hash Table

A map stores key–value pairs, allowing quick lookups by key. Ideal for fast retrieval without scanning all elements. Example: a user database mapping usernames to account details.

```mermaid
graph TD
    A[Map / Hash Table]
    A --> B["Insert: O(1) avg"]
    A --> C["Search: O(1) avg"]
    A --> D["Delete: O(1) avg"]
    A --> E["Example: User database storing profile information"]
```

```mermaid
graph TB
    K1[Key1] --> V1[Value1]
    K2[Key2] --> V2[Value2]
    K3[Key3] --> V3[Value3]
    subgraph Bucket1
        K1
    end
    subgraph Bucket2
        K2
    end
    subgraph Bucket3
        K3
    end
    classDef map fill:#fdf2e9,stroke:#333,stroke-width:1px;
    class K1,K2,K3,V1,V2,V3 map;
```
