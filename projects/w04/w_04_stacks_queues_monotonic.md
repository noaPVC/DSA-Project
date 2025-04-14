# Week 04: Stacks, Queues & Monotonic Patterns

## Purpose

This week is focused on mastering abstract linear data structures — stacks and queues — and learning how monotonic structures can be applied to optimize greedy and sliding window problems. These are crucial in parsing, scheduling, histogram problems, and many dynamic scenarios.

---

## Stacks (Days 1–2)

### 1. Concepts
- LIFO (Last-In-First-Out) structure
- Stack implementation using lists or `collections.deque`
- Common operations: `push`, `pop`, `peek`, `isEmpty`

### 2. Core Applications
- Balancing parentheses
- Undo/redo functionality
- Evaluation of postfix/prefix/infix expressions
- Backtracking algorithms
- Function call stack (recursion model)

### 3. Design Problems
- **Min Stack**: support retrieving the minimum in constant time
- **Implement Queue using Stacks**: simulate FIFO using two LIFOs

---

## Queues (Day 3)

### 1. Concepts
- FIFO (First-In-First-Out) structure
- Queue implementation using `collections.deque`
- Operations: `enqueue`, `dequeue`, `peek`, `isEmpty`

### 2. Core Applications
- BFS (Breadth-First Search) traversal
- Task scheduling, resource sharing
- Sliding window processing
- Producer-consumer systems

### 3. Design Problems
- **Circular Queue**: fixed-size queue that wraps around
- **Implement Stack using Queues**

---

## Monotonic Structures (Days 4–5)

### 1. Monotonic Stack
- Stack where elements are strictly increasing or decreasing
- Used to maintain order while solving in linear time
- Applications:
  - Next Greater Element
  - Largest Rectangle in Histogram
  - Daily Temperatures

### 2. Monotonic Queue
- Useful in sliding window max/min problems
- Keeps elements sorted while ensuring max/min is always at front

### 3. Design Insights
- Index-based storage vs value-based
- Tracking position and state with auxiliary arrays

---

## Sliding Window Pattern (Day 6)

### 1. Basics
- Move two pointers (start, end) to define a window over array/string
- Optimize subarray/subsequence computations
- Maintain running state (sum, max, frequency)

### 2. Variants
- Fixed window vs dynamic window
- Conditional shrinking: when to advance left pointer
- Use with hashmaps and sets for substring/array constraints

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Stack basics and usage patterns (postfix eval, matching symbols) |
| **2** | Design problems: Min Stack, Stack using Queues |
| **3** | Queue usage, BFS-like problems, task queues |
| **4** | Monotonic stacks: daily temps, next greater element |
| **5** | Monotonic queues: sliding window max/min |
| **6** | Full review of sliding window strategies |
| **7** | Recap + timed problem set + strategy consolidation |

---

## Practice Problem Ideas

### Stacks
- Valid Parentheses
- Min Stack
- Evaluate Reverse Polish Notation
- Asteroid Collision
- Remove K Digits

### Queues
- Implement Stack Using Queues
- Number of Recent Calls
- Perfect Squares (BFS)
- Rotting Oranges

### Monotonic Structures
- Daily Temperatures
- Next Greater Element I/II
- Largest Rectangle in Histogram
- Sliding Window Maximum

---

## Self-Check Questions

- Can I simulate stack and queue operations without using built-ins?
- Can I identify problems that can be transformed into monotonic patterns?
- Do I know when to use a queue over a stack and vice versa?
- Can I track indices and states efficiently in sliding window contexts?
- Can I explain why certain problems require a monotonic approach?

---

## Weekly Outcome

By the end of this week, you should:
- Be proficient with stack and queue manipulation
- Understand real-world applications of monotonic stacks and queues
- Efficiently solve sliding window problems using these tools
- Recognize linear-time optimization patterns in dynamic sequences

