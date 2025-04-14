# Week 07: Graph Traversals & Representations

## Purpose

Graphs generalize connections and relationships, enabling modeling of networks, dependencies, and reachability. This week establishes the core of graph-based thinking — exploring how graphs are represented, traversed, and analyzed using fundamental search techniques.

---

## Graph Foundations (Days 1–2)

### 1. Definitions & Types
- Vertex, edge, degree, path, cycle, component
- **Directed vs Undirected**
- **Weighted vs Unweighted**
- **Cyclic vs Acyclic**
- Dense vs sparse graphs

### 2. Representations
- **Adjacency List** (dictionary or array of lists): efficient for sparse graphs
- **Adjacency Matrix**: efficient for edge lookup, dense graphs
- **Edge List**: useful for sorting and Kruskal's algorithm

### 3. Input/Output Modeling
- Parsing edge lists into adjacency structures
- Handling 0-based vs 1-based indexing
- Graph traversal templates

---

## Depth-First Search (DFS) (Day 3)

### 1. Recursive DFS
- Pre-order/post-order visitation
- Maintain visited set
- Detecting cycles, checking connectivity

### 2. Iterative DFS
- Using explicit stack instead of recursion
- Parent tracking
- Backtracking strategies

### 3. Applications
- Connected components
- Path finding
- Tree traversal analogy

---

## Breadth-First Search (BFS) (Day 4)

### 1. BFS Mechanics
- Queue-based traversal
- Visited state per node
- Level-by-level exploration

### 2. Applications
- Shortest path in unweighted graphs
- Bipartite checking
- Spread or influence simulation

### 3. BFS vs DFS
- When to use each (path length, memory, structure)
- DFS explores depth; BFS explores breadth

---

## Cycle Detection & Topological Sort (Days 5–6)

### 1. Cycle Detection
- **Undirected**:
  - DFS with parent tracking
  - Union-Find (covered later)
- **Directed**:
  - DFS with visitation states: unvisited, visiting, visited
  - Detect back edges

### 2. Topological Sort
- **Kahn’s Algorithm**:
  - Track in-degree, queue nodes with zero in-degree
- **DFS-Based Toposort**:
  - Post-order stack, reverse for valid order

### 3. Applications
- Course scheduling
- Build system dependencies
- Job execution ordering

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Graph types, adjacency list/matrix representations |
| **2** | Edge list parsing, basic modeling, intro to traversal |
| **3** | DFS recursive/iterative traversal, visited tracking |
| **4** | BFS traversal and shortest path in unweighted graphs |
| **5** | Cycle detection (directed and undirected graphs) |
| **6** | Topological sort: DFS and Kahn’s algorithm |
| **7** | Review: simulate traversals on example graphs |

---

## Practice Problem Ideas

### Representation & Traversal
- Clone Graph
- Number of Connected Components
- Number of Islands
- Matrix Flood Fill (DFS/BFS hybrid)
- Graph Valid Tree

### BFS Applications
- Rotten Oranges
- Shortest Path in Binary Matrix
- Word Ladder I/II
- Open the Lock

### DFS Applications
- Course Schedule I/II
- Detect Cycle in Directed Graph
- Find Eventual Safe States
- Connected Components

---

## Self-Check Questions

- Can I correctly model a graph from edge input?
- Do I know when to use DFS vs BFS for a task?
- Can I implement cycle detection for both directed and undirected graphs?
- Do I understand how Kahn’s algorithm works with in-degree tracking?
- Can I trace a full traversal manually for correctness?

---

## Weekly Outcome

By the end of this week, you should:
- Be fluent in DFS and BFS traversal patterns
- Understand multiple graph representations and when to use each
- Implement topological sorting and detect cycles in both graph types
- Be ready to tackle path-finding and MST algorithms in Week 8