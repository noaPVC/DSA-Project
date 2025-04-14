# Week 09: Advanced Graph Algorithms

## Purpose

This week focuses on advanced graph problems involving **strongly connected components (SCCs)**, **bridges**, **articulation points**, and **graph connectivity**. These algorithms form the basis for understanding deeper properties of directed and undirected graphs, especially in system design, dependency resolution, and critical network analysis.

---

## Strongly Connected Components (SCCs) (Days 1–2)

### 1. Definition
- In a directed graph, a strongly connected component is a maximal set of nodes such that **every node is reachable from every other**.

### 2. Kosaraju’s Algorithm
- Step 1: Do DFS and record post-order (finish time) stack
- Step 2: Reverse all edges (transpose graph)
- Step 3: DFS in order of stack to collect components

### 3. Tarjan’s Algorithm
- Single DFS pass
- Uses low-link values to detect component roots
- Efficient and elegant; recursive stack structure

### 4. Applications
- Detecting cycles in dependency graphs
- Condensing large graphs into DAGs of components
- Finding circular references

---

## Bridges & Articulation Points (Days 3–4)

### 1. Definitions
- **Bridge**: An edge whose removal increases the number of connected components
- **Articulation Point**: A node whose removal increases the number of components

### 2. Bridge Finding (Tarjan-like DFS)
- Track discovery time and lowest reachable ancestor
- If `low[v] > disc[u]`, then edge (u,v) is a bridge

### 3. Articulation Point Finding
- For each node, check if removing it disconnects subtrees
- Special handling for root node (must have ≥2 children to be articulation point)

### 4. Applications
- Identifying vulnerable connections
- Network fault tolerance
- Traffic or server routing bottlenecks

---

## Union-Find & Disjoint Set Union (DSU) (Day 5)

### 1. Core Concepts
- Efficiently track connected components
- Supports two operations:
  - `find(x)`: returns the representative of x
  - `union(x, y)`: merges sets containing x and y

### 2. Optimizations
- **Path Compression**: flatten trees during `find`
- **Union by Rank/Size**: attach smaller tree under root of larger

### 3. Applications
- Kruskal’s MST
- Connected components in offline queries
- Dynamic connectivity

---

## Advanced Applications (Day 6)

### 1. Critical Connections in a Network
- Identify bridges in a network graph

### 2. 2-SAT and Implication Graphs (optional)
- Represent logic constraints as graph
- Use SCCs to determine satisfiability

### 3. Offline Queries and DSU on Trees (bonus/extra)
- Binary lifting + DSU for dynamic subtree queries

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Strongly connected components: Kosaraju’s algorithm |
| **2** | Tarjan’s algorithm for SCCs, low-link value intuition |
| **3** | Bridge detection with DFS timestamp tracking |
| **4** | Articulation points and graph vulnerability |
| **5** | Union-Find: disjoint sets, path compression, union by rank |
| **6** | Critical connection problems and SCC applications |
| **7** | Recap + manual graph tracing + review with visualization |

---

## Practice Problem Ideas

### SCCs
- Find Strongly Connected Components
- Minimum Edges to Make Graph Strongly Connected
- 2-SAT Satisfiability

### Bridges & Articulation Points
- Critical Connections in a Network
- Articulation Points in Graph
- Biconnected Components

### Union-Find Applications
- Redundant Connection
- Number of Connected Components
- Accounts Merge
- Satisfiability of Equality Equations

---

## Self-Check Questions

- Can I explain the difference between bridges and articulation points?
- Do I understand how low-link values guide component structure?
- Can I trace Tarjan’s algorithm step-by-step on a small graph?
- Do I know when to use DFS-based analysis vs Union-Find?
- Can I build intuition for cyclic structure in directed graphs?

---

## Weekly Outcome

By the end of this week, you should:
- Identify and extract SCCs in directed graphs using Kosaraju or Tarjan
- Detect bridges and articulation points in undirected graphs
- Use Union-Find to efficiently manage component sets
- Understand graph vulnerabilities and connectedness at a deeper level