# Linked-List-in-Cpp

# Aim

To study and implement the concept of a singly linked list in C++, including node creation, manual node linking, and insertion at head, and to understand how traversal and display operations work.

# Software Used

Compiler: GNU GCC (g++)

IDE: Visual Studio Code

Operating System: Windows/Linux

# Theory

A linked list is a linear data structure in which elements, called nodes, are stored at non-contiguous memory locations and are connected by pointers. Each node contains:

    Data field — stores the actual information.
    
    Pointer field — stores the address of the next node.

A singly linked list starts with a head pointer that points to the first node. The last node’s pointer is set to NULL to indicate the end of the list.

Key Characteristics:

    Dynamic size (can grow/shrink during runtime).
    
    Efficient insertion and deletion at head or middle (no shifting required).
    
    Traversal is sequential; no random access like arrays.

Benefits:

    Flexible memory usage.
    
    Insertions/deletions are efficient at the head.
    
    Useful for dynamic data structures like stacks, queues, graphs, etc.

Limitations:

    Requires extra memory for pointers.
    
    Sequential access only; no indexing.
    
    Improper pointer handling can cause memory leaks.

# Algorithms

# 1. Node Creation (Linked List 1.cpp)

Algorithm:

    Start the program.
    
    Define a Node structure/class with two fields:
    
      val (data field).
      
      next (pointer to the next node).
    
    Write a constructor that initializes the node with:
    
      val = data (given value).
      
      next = NULL (no next node yet).
    
    In main:
    
      Create a node dynamically with a value.
      
      Print its data and next pointer value.
    
    End the program.

Expected Output: Data of the node followed by NULL (or 0).

# 2. Manual Linking of Nodes and Traversal (Linked List 2.cpp)

Algorithm:

    Start the program.
    
    Define a Node structure/class with fields val and next.
    
    Write a constructor to initialize data and set next = NULL.
    
    In main:
    
      Create three nodes with values.
      
      Link them: first node → second node → third node.
      
      Keep the third node’s next = NULL.
    
    Create a temporary pointer temp = head (first node).
    
    While temp is not NULL:
    
      Print temp->val.
      
      Move to the next node (temp = temp->next).
      
    End the program.

Expected Output: Sequence of node values (e.g., 10 20 30).

# 3. Insertion at Head and Display (Linked List 3.cpp)

Algorithm:

    Start the program.
    
    Define a Link class with fields:
    
      data (node’s value).
      
      next (pointer to next node).
    
    Write a constructor to initialize data and set next = NULL.
    
    Define a function insert_head(head, data):
    
      Create a new node with given data.
      
      Set new node’s next to current head.
      
      Update head to point to new node.
      
    Define a function disp(head) to display the list:
    
      Start from head.
      
      While the node is not NULL:
      
        Print its data.
        
        Move to next node.
      
      Print NULL at the end.
    
    In main:
    
      Initialize list as empty (head = NULL).
      
      Call insert_head with values (e.g., 30, 32, 35).
      
      After each insertion, call disp to show updated list.
    
    End the program.

Expected Output:

30 NULL  
32 30 NULL  
35 32 30 NULL  

# Conclusion

Through these three programs, the basics of linked lists were implemented and understood:

    Node creation showed how a node stores data and a pointer.
    
    Manual linking demonstrated chaining nodes together and traversing them.
    
    Insertion at head illustrated how new elements can be efficiently added at the beginning of the list.

This experiment clarified the working of dynamic memory, pointers, and sequential data access in C++. Linked lists provide a strong foundation for more advanced structures like stacks, queues, and graphs, making them an essential concept in data structures.
