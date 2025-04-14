# Week 03: Linked Lists + Recursion

## Purpose

This week covers recursive thinking and linked list manipulation — both are cornerstones of algorithmic problem solving. Linked lists teach pointer logic, node structures, and memory layout. Recursion builds understanding of call stacks, base cases, and backtracking.

---

## Linked Lists (Days 1–3)

### 1. Fundamentals
- **Node structure**: value + pointer to next (and previous)
- **Types**:
  - Singly linked list
  - Doubly linked list
  - Circular linked list
- **Traversal**: linear scan using `current = current.next`

### 2. Operations
- Insertion: at head, tail, or middle
- Deletion: by value, position
- Search: by value, index
- Reversal (in-place): iterative pointer manipulation
- Cycle detection (Floyd's Tortoise and Hare)

### 3. Variants & Applications
- Merge two sorted lists
- Intersecting linked lists
- Detect and find entry point of a loop
- Copy list with random pointer (deep copy)

---

## Recursion (Days 4–5)

### 1. Core Principles
- Base case and recursive case
- Recursive tree visualization
- Stack overflow, depth limits, Python recursion limit

### 2. Problem Types
- Mathematical: factorial, Fibonacci, exponentiation
- List recursion: reverse list, sum of elements
- Divide and Conquer: merge sort, binary search (recursive)
- Backtracking: permutations, subsets, combinations

### 3. Tail vs Head Recursion
- Tail: work done during unwinding
- Head: work done during stack building

### 4. Debugging Recursion
- Print trace/logs
- Use diagrams to model state
- Add memoization if overlapping subproblems occur

---

## Combined Concepts (Day 6)

### 1. Recursive Linked List Problems
- Reverse list recursively
- Detect palindrome in a linked list recursively
- Add two numbers represented as linked lists

### 2. Backtracking & Tree Traversals (Foreshadowing Trees)
- DFS-like recursion
- Handling state rollback and pruning paths

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Singly and doubly linked list traversal and construction |
| **2** | Deletion, insertion, reversal (in-place) |
| **3** | Cycle detection, merging, dummy nodes, real-world problems |
| **4** | Base vs recursive cases, writing clean recursive logic |
| **5** | Recursive applications: backtracking, Fibonacci, binary recursion |
| **6** | Recursive solutions to linked list problems |
| **7** | Review: draw call stacks, simulate pointer behavior, refactor |

---

## Practice Problem Ideas

### Linked Lists
- Reverse Linked List
- Detect Cycle in Linked List
- Merge Two Sorted Lists
- Add Two Numbers
- Intersection of Two Linked Lists
- Copy List with Random Pointer

### Recursion
- Permutations
- Subsets
- Generate Parentheses
- Climbing Stairs
- Letter Combinations of Phone Number

---

## Self-Check Questions

- Can I simulate linked list operations without relying on array indices?
- Do I understand the recursive call stack for each case?
- Can I identify and write clear base cases?
- Can I explain how recursion unwinds?
- Can I refactor iterative problems into recursive versions (and vice versa)?

---

## Weekly Outcome

By the end of this week, you should:
- Comfortably create, manipulate, and debug linked lists
- Visualize and implement recursive logic
- Solve classic recursive and pointer-based problems
- Be ready to transition into tree-based recursion next week

