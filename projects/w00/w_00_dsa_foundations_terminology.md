# Week 00: DSA Foundations & Terminology — The "Hello World" of This Roadmap

## Purpose

Before diving into data structures and algorithms (DSA), it’s essential to build a strong foundation of terminology and conceptual understanding. This pre-week sets the stage with universal principles, regardless of programming language, and helps you build the mental model to talk about and reason about DSA precisely.

---

## Why Learn DSA?

- **Efficiency**: Knowing the right data structure or algorithm reduces computation time and memory use.
- **Problem Solving**: DSA provides patterns for approaching complex coding challenges logically.
- **Interviews**: Most technical interviews test core DSA skills.
- **Scalability**: DSA underpins performance in real-world software and systems.

---

## Core Concepts & Terminology

### 1. Data Structure
A way to **organize and store data** so it can be accessed and modified efficiently.

Types:
- **Linear**: Array, Linked List, Stack, Queue
- **Non-linear**: Tree, Graph, Trie
- **Hash-based**: Hash Table, Hash Set, Map

### 2. Algorithm
A **step-by-step procedure** to solve a problem or perform a task.

Types:
- **Sorting**: Quick Sort, Merge Sort, Radix Sort
- **Searching**: Binary Search, DFS, BFS
- **Optimization**: Dynamic Programming, Greedy
- **Graph algorithms**: Dijkstra, Prim, Kruskal, Tarjan

---

## Time & Space Complexity

### Big O Notation
Describes the **worst-case** performance as input size grows.

| Complexity | Description               | Example                  |
|------------|---------------------------|--------------------------|
| O(1)       | Constant time              | Accessing array element  |
| O(log n)   | Logarithmic                | Binary search            |
| O(n)       | Linear                     | Iterating over array     |
| O(n log n) | Linearithmic               | Merge sort               |
| O(n^2)     | Quadratic                  | Nested loops             |
| O(2^n)     | Exponential                | Brute-force DP recursion |
| O(n!)      | Factorial                  | Permutations             |

**Space complexity** works the same way, but refers to **memory usage**.

---

## Recursion
A function that calls itself to solve smaller instances of the problem.

Key terms:
- **Base Case**: Stops the recursion.
- **Recursive Case**: Continues toward the base.
- **Call Stack**: Tracks active function calls.

---

## Overlapping Subproblems
Subparts of a problem are solved multiple times — ideal for **dynamic programming**.

---

## Common Patterns and Terms (Across All 10 Weeks)

| Term | Definition |
|------|------------|
| **Pointer** | A reference to another memory location, used conceptually even in Python |
| **Traversal** | Visiting every node/item in a structure |
| **Subarray/Subsequence** | Contiguous vs non-contiguous elements of an array or string |
| **Greedy Choice** | A locally optimal decision aimed at global optimality |
| **Memoization** | Cache results of function calls (top-down DP) |
| **Tabulation** | Iteratively building up results (bottom-up DP) |
| **Heap** | A binary tree-based priority queue (min/max) |
| **Backtracking** | Recursively exploring all possible states |
| **Monotonic Stack** | A stack that maintains increasing/decreasing order |
| **Cycle** | A loop in a graph where you can return to the starting node |
| **Connected Component** | A group of nodes in a graph where each node is reachable from any other |
| **Prefix Sum** | Running total up to index i, used in subarray calculations |
| **Bitmask** | A binary encoding of set membership or state |
| **Topological Sort** | Ordering nodes in a directed graph such that dependencies come first |
| **Union-Find** | A data structure to track disjoint sets, used in Kruskal’s MST |
| **Trie** | A prefix tree structure for storing strings and queries efficiently |

---

## Visual Thinking in DSA

Think in terms of:
- **Diagrams**: Arrays, trees, graphs
- **State transitions**: Especially for DP
- **Flowcharts**: Helpful for recursive decision making

---

## How This Foundation Helps

Understanding these terms equips you to:
- Speak clearly and accurately about problem-solving approaches
- Write more efficient, readable code
- Collaborate on complex algorithmic systems
- Master interview patterns and beyond

---

## Your Goals for Week 00

- Review this glossary and revisit it throughout the roadmap
- Practice identifying complexity in code you write
- Diagram out recursion trees and DP tables
- Translate problems into state-based models

Let’s now move into Week 01 — where Python basics meet real problem solving.
