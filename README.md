# Experiment 17: Linked Lists in C++

---

## Aim
To study and implement the concept of **Linked Lists** in C++ by performing the following operations:  
1. Creating nodes and linking them.  
2. Parsing through a node using pointers.  
3. Inserting elements at the head end of a linked list.  
4. Inserting elements at the tail end of a linked list.  

---

## Tools
- **Programming Language**: C++  
- **Compiler**: g++ / Turbo C++ / MinGW or any standard C++ compiler  
- **IDE/Editor**: VS Code, Code::Blocks, or any preferred editor  
- **Operating System**: Windows / Linux / macOS  

---

## Theory
A **Linked List** is a linear data structure where elements (nodes) are stored in non-contiguous memory locations. Each node contains:  
1. **Data** – The value stored in the node.  
2. **Pointer (next)** – A reference to the next node in the sequence.  

Unlike arrays, linked lists provide **dynamic memory allocation**, meaning their size can grow or shrink at runtime.  

### Types of Linked Lists:
- **Singly Linked List**: Each node points to the next node.  
- **Doubly Linked List**: Each node has two pointers (next and previous).  
- **Circular Linked List**: Last node points back to the first node.  

For this experiment, we focus on **singly linked lists**.  

### Advantages:
- Dynamic size (no fixed limit).  
- Efficient insertion and deletion compared to arrays.  

### Disadvantages:
- Sequential access (slower than arrays for searching).  
- Requires extra memory for pointers.  

---

## Algorithm

### A. Creating Nodes and Linking Them
1. Define a `struct Node` containing `data` and `next` pointer.  
2. Allocate memory dynamically for each node.  
3. Assign data to each node.  
4. Link the nodes by setting the `next` pointer of one node to another.  
5. Set the last node’s `next` as `NULL` to indicate the end.  

---

### B. Parsing Through a Node Using Pointers
1. Start with the head pointer of the linked list.  
2. Use a temporary pointer to traverse.  
3. While the current node is not `NULL`:  
   - Print the node’s data.  
   - Move to the next node.  
4. Stop when the end of the list is reached.  

---

### C. Inserting Linked List Elements from the Head End
1. Create a new node.  
2. Assign data to the new node.  
3. Set the new node’s `next` to the current head.  
4. Update the head pointer to the new node.  
5. Repeat as required.  

---

### D. Inserting Linked List Elements from the Tail End
1. Create a new node.  
2. Assign data to the new node and set its `next = NULL`.  
3. If the list is empty, make this node the head.  
4. Else, traverse the list until the last node.  
5. Set the last node’s `next` pointer to the new node.  

---

## Functions Used
- **`createNode(data)`** – Dynamically allocates memory for a new node.  
- **`display(head)`** – Traverses the list and displays node data.  
- **`insertHead(head, data)`** – Inserts a new node at the head.  
- **`insertTail(head, data)`** – Inserts a new node at the tail.  

---

## Conclusion
From this experiment, we achieved the following:  
1. Learned how to create and link nodes dynamically using pointers.  
2. Understood how to traverse (parse) a linked list sequentially.  
3. Implemented insertion at both the **head** and **tail** of the list.  
4. Understood that linked lists provide **dynamic memory allocation**, unlike arrays.  

This experiment demonstrated the foundation of linked lists, which serve as the basis for advanced data structures like stacks, queues, and trees.  
