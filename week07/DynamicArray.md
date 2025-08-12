## Dynamic Array

A **Dynamic Array** stores elements in contiguous memory but automatically resizes when it reaches capacity (often doubling its size).  
It allows **O(1)** access by index and efficient appends, but inserting at the beginning or middle requires shifting elements.  
Dynamic arrays are useful when you need quick random access and occasional resizing, such as maintaining a live playlist of songs that can be added or removed.

```mermaid
graph TD
    A[Dynamic Array]
    A --> B["Insert at beginning: O(n)"]
    A --> C["Insert at end: O(1) amortized"]
    A --> D["Access by index: O(1)"]
    A --> E["Search by value: O(n)"]
    A --> F["Example: Dynamic playlist where songs can be added/removed"]
```

The diagram above shows the time complexities and a typical use case.

Below is a visual representation of how elements are stored sequentially in a dynamic array.

mermaid
Copy
Edit


```mermaid
graph LR
    A0[0] --- A1[1] --- A2[2] --- A3[3] --- A4[4] --- AX[...]
    classDef array fill:#f9f9f9,stroke:#333,stroke-width:1px;
    class A0,A1,A2,A3,A4,AX array;
```