# Week 05: Trees & Binary Search Trees (BSTs)

## Purpose

Trees introduce a hierarchical structure that underpins recursion, binary operations, and efficient search. Understanding traversal strategies and binary search tree properties unlocks more advanced structures and problem-solving approaches across algorithms, parsing, indexing, and dynamic programming.

---

## Tree Fundamentals (Days 1–2)

### 1. Structure and Terminology
- Node, edge, root, child, parent, leaf, internal node, height, depth, level
- Binary tree: each node has up to two children
- Full, perfect, complete, balanced trees — definitions and properties

### 2. Representations
- Node class with left/right pointers
- Tree from array (e.g., heap-style)
- Recursive vs iterative construction

### 3. Traversal Types
- **Depth-First**:
  - Inorder: left → root → right
  - Preorder: root → left → right
  - Postorder: left → right → root
- **Breadth-First**:
  - Level-order traversal using queue
  - Zigzag level-order (alternating direction)
- Recursive vs Iterative (stack/queue-based)

---

## Binary Search Trees (BSTs) (Days 3–4)

### 1. BST Properties
- Left child < root < right child
- Sorted in-order traversal
- Average height: O(log n); worst case: O(n)

### 2. BST Operations
- Search for a node
- Insert a new value
- Delete a node: three-case logic (0, 1, or 2 children)
- Validate BST recursively (range or in-order)

### 3. Traversal Usage
- Preorder to serialize a tree
- Inorder to rebuild BST
- Use DFS to compute height, balance, diameter

---

## Tree Construction (Day 5)

### 1. Build from Traversal Orders
- Inorder + Preorder = unique tree
- Inorder + Postorder = unique tree
- Use recursive slicing or index maps

### 2. Serialization / Deserialization
- Save tree to string (preorder with null markers)
- Restore from string using queue/indexed recursion

### 3. Convert Between Trees and Arrays
- Build balanced BST from sorted array
- Flatten binary tree into a list (e.g. for LCA problems)

---

## Tree Algorithms (Day 6)

### 1. Structural Analysis
- Max Depth / Min Depth
- Balanced Tree Check (height-balance property)
- Tree Diameter (longest path through tree)

### 2. Tree Search Variants
- Lowest Common Ancestor (LCA)
- Path sum problems
- Mirror and invert operations
- Subtree matching

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Tree terminology, basic structure, recursive node class |
| **2** | Traversals (inorder, preorder, postorder, level-order) — recursive and iterative |
| **3** | BST properties and operations: insert, delete, validate |
| **4** | BST edge cases, in-order successorship, duplicate handling |
| **5** | Construct trees from traversal orders, serialize/deserialize trees |
| **6** | Tree depth, balance check, LCA, and path sum problems |
| **7** | Recap + drawing exercises + traversal pattern review |

---

## Practice Problem Ideas

### Tree Traversals
- Binary Tree Inorder Traversal
- Binary Tree Preorder Traversal
- Binary Tree Postorder Traversal
- Level Order Traversal
- Zigzag Level Order Traversal

### BSTs
- Validate Binary Search Tree
- Insert into a Binary Search Tree
- Delete Node in a BST
- Kth Smallest Element in a BST
- Lowest Common Ancestor of BST

### Tree Algorithms
- Maximum Depth of Binary Tree
- Diameter of Binary Tree
- Path Sum I/II/III
- Serialize and Deserialize Binary Tree
- Construct Binary Tree from Traversal

---

## Self-Check Questions

- Can I clearly differentiate each tree type (complete, balanced, perfect)?
- Can I write and visualize all four major tree traversals?
- Do I understand how BSTs guarantee faster search compared to arrays?
- Can I reconstruct a tree from traversal data?
- Am I able to explain recursive logic for both traversal and construction?

---

## Weekly Outcome

By the end of this week, you should:
- Understand and implement binary tree structures and traversal strategies
- Perform all key operations on binary search trees
- Translate traversal order into construction logic and recursive processes
- Solve path-based and structural problems using trees