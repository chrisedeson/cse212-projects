## Queue

A **Queue** is a linear data structure that follows the First-In-First-Out (FIFO) principle.  
Elements are added (enqueued) at the rear and removed (dequeued) from the front.  
It’s ideal for situations where processing happens in order of arrival.  
A common example is a print job management system, where the first document sent to the printer is processed first.

```mermaid
graph TD
    A[Queue]
    A --> B["Enqueue: O(1)"]
    A --> C["Dequeue: O(1)"]
    A --> D["Peek: O(1)"]
    A --> E["Example: Print job management system"]
```

The diagram above shows the operation complexities and a typical use case.

Below is a visual representation of a queue with elements ordered from front to rear.

```mermaid
graph LR
    Front[Front] --> Q1[Item 1] --> Q2[Item 2] --> Q3[Item 3] --> Rear[Rear]
    classDef queue fill:#f4ecf7,stroke:#333,stroke-width:1px;
    class Front,Q1,Q2,Q3,Rear queue;
```