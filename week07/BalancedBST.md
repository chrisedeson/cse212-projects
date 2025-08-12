## Balanced Binary Search Tree (BST)

A **Balanced BST** is a binary search tree that keeps its height minimal by ensuring the difference in height between the left and right subtrees is small (often at most 1).  
This balance property keeps operations efficient — typically `O(log n)` for insertion, search, and deletion.  
Balanced BSTs are useful when you need fast lookups while maintaining a sorted structure, such as in leaderboards or autocomplete systems.

```mermaid
graph TD
    A[Balanced BST]
    A --> B["Insert: O(log n)"]
    A --> C["Search: O(log n)"]
    A --> D["Delete: O(log n)"]
    A --> E["Traversal: O(n)"]
    A --> F["Example: Autocomplete in search engines"]
```

The diagram above summarizes the time complexity and a common use case.

Below is a visual structure of a balanced BST showing the relationship between the root, its subtrees, and child nodes.

```mermaid
graph TD
    R[Root]
    R --> L[Left Subtree]
    R --> Ri[Right Subtree]
    L --> LL[Left Child]
    L --> LR[Right Child]
    Ri --> RL[Left Child]
    Ri --> RR[Right Child]
    classDef bst fill:#ebf5fb,stroke:#333,stroke-width:1px;
    class R,L,Ri,LL,LR,RL,RR bst;
```