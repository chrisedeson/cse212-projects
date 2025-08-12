## Linked List (Doubly-linked)

A **Doubly-linked list** is a linear data structure where each node contains data and two pointers: one to the previous node and one to the next node.  
It allows efficient insertion and deletion at both ends or in the middle without shifting other elements.  
However, accessing an element by index requires traversal from the head or tail, making it **O(n)**.  
A practical example is a browser’s forward/backward history, where you can move in either direction through visited pages.

```mermaid
graph TD
  subgraph Info["Linked List — Doubly linked"]
    B["Insert at beginning: O(1)"]
    C["Insert at end: O(1) with tail pointer"]
    D["Access by index: O(n)"]
    E["Search by value: O(n)"]
    F["Example: Browser history navigation"]
  end
```
The diagram above summarizes the time complexities and a common real-world use case.

Below is a visual structure of a doubly-linked list showing nodes and bidirectional pointers.

```mermaid
graph LR
    N1["Prev<br>Data1<br>Next"] <--> N2["Prev<br>Data2<br>Next"] <--> N3["Prev<br>Data3<br>Next"]
    classDef node fill:#fef9e7,stroke:#333,stroke-width:1px;
    class N1,N2,N3 node;
```