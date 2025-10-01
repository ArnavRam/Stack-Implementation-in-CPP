# Experiment 18 - Stack implementation using array

---

## Aim
- To study and implement **Stack** operations in C++ using an array.
- To understand the LIFO (Last In, First Out) principle of data management.

---

## Tools Used
- Visual Studio Code
- MinGW-w64 with g++ Compiler

---

## Theory
A **Stack** is a linear data structure that follows the **LIFO (Last In, First Out)** principle. The element that is inserted last is the first one to be removed, similar to a stack of plates. A stack is managed with a single pointer:
- **`top`:** Points to the most recently inserted element in the stack.

### Key Characteristics
- **LIFO Order:** The last element added is the first to be removed.
- **Restricted Access:** Insertions (push) and deletions (pop) happen only at the `top`.
- **Overflow/Underflow:** Overflow occurs when an attempt is made to push an element onto a full stack. Underflow occurs when an attempt is made to pop an element from an empty stack.

---

## Algorithm / Logic
1.  **Start**
2.  Initialize an integer array `stack_array` of a fixed `MAX` size.
3.  Initialize `top = -1`.
4.  Display a menu with options: 1. Push, 2. Pop, 3. Display, 4. Exit.
5.  Use a loop to repeatedly ask the user for their choice until they select Exit.

    -   **Case 1: Push**
        -   Check if the stack is full (`top == MAX - 1`). If so, print "Stack Overflow".
        -   Otherwise, prompt the user for a value to insert.
        -   Increment `top` by 1.
        -   Store the value at `stack_array[top]`.

    -   **Case 2: Pop**
        -   Check if the stack is empty (`top == -1`). If so, print "Stack Underflow".
        -   Otherwise, display the element at `stack_array[top]`.
        -   Decrement `top` by 1.

    -   **Case 3: Display**
        -   Check if the stack is empty. If so, print "Stack is empty".
        -   Otherwise, use a `for` loop to iterate from `top` down to `0` and print each element of the stack.

    -   **Case 4: Exit**
        -   Terminate the program.

6.  **End**

---

## Conclusion
The Stack is a fundamental data structure that strictly adheres to the LIFO principle. This experiment demonstrated how to implement a stack using an array and manage its state with a `top` pointer. The core operations of push (insertion at the top) and pop (deletion from the top) were successfully implemented, along with checks for overflow and underflow conditions. Stacks are essential for managing function calls (the call stack), parsing expressions, backtracking algorithms, and many other applications in computer science.
