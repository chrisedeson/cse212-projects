## Stack

A **Stack** is a linear data structure that follows the Last-In-First-Out (LIFO) principle.  
Elements are added (pushed) and removed (popped) only from the top of the stack.  
It’s efficient for scenarios where you need to reverse order or track nested operations.  
A common example is the undo/redo system in a text editor, where the most recent change is the first to be undone.

```mermaid
graph TD
    A[Stack]
    A --> B["Push: O(1)"]
    A --> C["Pop: O(1)"]
    A --> D["Peek: O(1)"]
    A --> E["Example: Undo/Redo in text editor"]
```

The diagram above shows operation complexities and a real-world example.

Below is a visual representation of a stack with the top element shown first.


```mermaid
graph TD
    Top[Top] --> E1[Item 1]
    E1 --> E2[Item 2]
    E2 --> E3[Item 3]
    classDef stack fill:#e8f8f5,stroke:#333,stroke-width:1px;
    class Top,E1,E2,E3 stack;
```