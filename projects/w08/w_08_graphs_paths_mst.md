# Week 08: Shortest Paths & Minimum Spanning Trees (MST)

## Purpose

This week deepens graph mastery by tackling **weighted graphs**. You'll explore algorithms for finding shortest paths (with and without constraints) and building optimal networks using minimum spanning trees. These techniques are critical in routing, optimization, logistics, and planning.

---

## Weighted Graphs (Day 1)

### 1. Representation
- Adjacency list with (neighbor, weight) tuples
- Edge list with weights (for Kruskal’s)
- Adjacency matrix with weights (dense graph use case)

### 2. Edge Weights
- Positive vs negative weights
- Uniform vs variable weights
- Real-world modeling: roads, costs, time, distance

---

## Dijkstra’s Algorithm (Day 2)

### 1. Goal
- Find shortest path from a source node to all others
- Only works with **non-negative edge weights**

### 2. Algorithm Overview
- Use priority queue (min-heap) to always expand nearest node
- Track shortest known distance per node
- Update neighbors with `min(current_cost + edge_cost)`

### 3. Optimization
- Use `heapq` (Python min-heap)
- Early stopping when destination is found

### 4. Applications
- GPS navigation
- Network packet routing
- Cheapest cost problems

---

## Bellman-Ford Algorithm (Day 3)

### 1. When to Use
- Graphs with **negative weights** (but no negative cycles)
- Not as fast as Dijkstra, but more flexible

### 2. Algorithm Overview
- Relax all edges **V - 1** times
- If you can still relax an edge on pass `V`, a negative cycle exists

### 3. Applications
- Detect arbitrage
- Shortest path in constrained environments

---

## Shortest Path Variants (Day 4)

### 1. Multi-Constraint Problems
- Cheapest Flights with K Stops
- Path with maximum probability
- Path minimizing risk, fuel, cost

### 2. Modifications of Dijkstra
- Add stop count, visited state, custom weight logic
- Use of multiple queues or states (multi-dimensional DP or (node, cost, hops) tuples)

### 3. Grid Problems as Graphs
- Minimum cost path in a grid
- Weighted shortest path in 2D matrix with obstacles

---

## Minimum Spanning Trees (MST) (Days 5–6)

### 1. MST Definition
- Subset of edges that connect all nodes with **minimal total weight**
- Tree (no cycles), covers all nodes

### 2. Kruskal’s Algorithm
- Sort edges by weight
- Greedily add edges using Union-Find to avoid cycles

### 3. Prim’s Algorithm
- Expand from one node using priority queue
- Add minimum weight edge connecting visited to unvisited node

### 4. Union-Find (Disjoint Set Union - DSU)
- Used in Kruskal’s to detect cycles
- Path compression and union by rank

### 5. Applications
- Network cabling with minimal cost
- Campus road design
- Clustering

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Weighted graph modeling and adjacency formats |
| **2** | Dijkstra’s algorithm and shortest path applications |
| **3** | Bellman-Ford algorithm and negative weight graphs |
| **4** | Constrained shortest paths and modified Dijkstra |
| **5** | MST overview, Kruskal’s algorithm, sorting edge lists |
| **6** | Prim’s algorithm, Union-Find data structure |
| **7** | Review: graph diagrams, path tracking, MST exercises |

---

## Practice Problem Ideas

### Shortest Path
- Dijkstra:
  - Network Delay Time
  - Path with Minimum Effort
- Bellman-Ford:
  - Cheapest Flights Within K Stops
  - Detect Negative Cycle
- Grid Path:
  - Minimum Cost to Reach Cell
  - Shortest Path in Weighted Grid

### MST & Union-Find
- Minimum Cost to Connect All Points
- Connecting Cities with Minimum Cost
- Kruskal’s vs Prim’s comparison
- Number of Connected Components
- Accounts Merge (DSU application)

---

## Self-Check Questions

- Do I understand how edge weights affect traversal order?
- Can I implement Dijkstra with a priority queue?
- Can I detect and interpret negative weight cycles with Bellman-Ford?
- Do I know when to use Kruskal vs Prim?
- Can I implement Union-Find with path compression?

---

## Weekly Outcome

By the end of this week, you should:
- Model and analyze weighted graphs confidently
- Implement and adapt Dijkstra and Bellman-Ford
- Solve real-world shortest path problems under constraints
- Build and analyze MSTs using Kruskal’s and Prim’s algorithms
