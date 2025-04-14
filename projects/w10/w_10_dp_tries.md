# Week 10: Dynamic Programming & Tries

## Purpose

This final week dives into two high-leverage tools in algorithmic problem-solving: **Dynamic Programming (DP)** and **Tries**. Both are considered "advanced" but crucial for mastering LeetCode hard problems, technical interviews, and real-world system design tasks involving optimization and search indexing.

Dynamic Programming is the art of identifying overlapping subproblems and reusing past results to avoid redundant computation. Tries are tree-based data structures that allow ultra-fast prefix-based querying and string classification.

---

## Dynamic Programming (DP)

### What is Dynamic Programming?
Dynamic Programming is a method for solving complex problems by breaking them down into simpler overlapping subproblems and solving each just once, storing their results (via memoization or tabulation).

Key characteristics:
- **Overlapping subproblems**: The same subproblem is solved multiple times in recursion
- **Optimal substructure**: An optimal solution to a problem contains the optimal solutions to its subproblems

### Two Main Flavors
1. **Top-Down (Memoization)**:
   - Recursive implementation with caching
   - Easy to write, mirrors brute-force
   - Useful when not all subproblems are needed
2. **Bottom-Up (Tabulation)**:
   - Iterative approach building from base cases
   - Often faster and avoids recursion stack limits
   - Easier to optimize for space

---

## Structuring DP (Days 1–2)

### 1. State Definition
- What parameters define the subproblem?
- How to uniquely identify a subproblem using a tuple of inputs?
- Typical states: index, target, capacity, remaining items, mask, coordinates

### 2. Transition Function
- How do you move from smaller subproblems to a larger one?
- Use recurrence relations or decision trees to derive transitions

### 3. Base Cases
- These anchor the recursion or iteration
- Start with the smallest valid inputs and grow from there

### 4. Space Optimization
- Reduce DP dimensions when only previous row/state is needed
- Use rolling arrays, variable swaps, or constant memory tricks

---

## Classic DP Patterns (Day 3)

### Fibonacci-like Recurrence
- `dp[i] = dp[i-1] + dp[i-2]`
- Problems: Climbing Stairs, Tiling problems

### 0/1 Knapsack
- `dp[i][w] = max(dp[i-1][w], dp[i-1][w-wt[i]] + val[i])`
- Problems: Subset sum, Partition equal subset sum, House Robber

### Longest Increasing Subsequence
- O(n^2) DP or O(n log n) with patience sorting
- Monotonic subsequence construction

### Matrix-Based DP
- Used in Edit Distance, LCS, Unique Paths
- Use 2D matrices to represent grid/match alignment

---

## Advanced DP (Day 4)

### Bitmask DP
- Represents state using binary digits
- Used when multiple elements need to be “visited” or “covered”
- Common in TSP, subset state problems, and DP on permutations

### DP on Trees
- Combine DP values of children recursively
- Problems: Longest Path in Tree, DP on rooted subtrees

### DP + Binary Search
- For optimization (e.g., LIS with patience sorting)
- Jump search on answer value

### Palindromic DP
- Substring is palindrome if s[i] == s[j] and s[i+1..j-1] is palindrome
- Used in palindrome partitioning, LPS

---

## Tries (Days 5–6)

### What is a Trie?
A Trie (prefix tree) is a tree-like data structure that stores strings character-by-character. Paths in the tree represent prefixes. It enables ultra-fast lookups, insertions, and prefix checks in O(length of word).

### Components of a Trie Node
- Children map: from char → next TrieNode
- End-of-word flag
- Optional: frequency counter, full-word storage, weight

### Basic Operations
- `insert(word)`
- `search(word)`
- `startsWith(prefix)`

### Variants
- **Compressed Tries (Radix Trees)**: Compress chains of single-child nodes
- **Suffix Tries / Automata**: Store all suffixes of a string (heavy memory use)
- **Trie of Trie**: Multi-level tries for dictionaries with meta-prefixing

---

## Trie + DFS and Backtracking (Day 6 continued)

Tries are often used with DFS for word search:
- Use the Trie for fast prefix validation
- Use DFS to explore the grid or string space
- Prune early when prefix not found
- Backtrack using visited sets or cell marking

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Intro to DP: state, transitions, recursion vs iteration |
| **2** | Classic patterns: climbing stairs, knapsack, matrix DP |
| **3** | Advanced techniques: LIS, LCS, tree DP, palindromic DP |
| **4** | Bitmask DP, TSP, partitioning, optimization techniques |
| **5** | Building a Trie: insert, search, prefix checking |
| **6** | DFS + Trie applications: Word Search II, Dictionary problems |
| **7** | Wrap-up review: summarize patterns, reflect on mastery, reinforce weak spots |

---

## Practice Problem Ideas

### DP
- Climbing Stairs
- House Robber I/II
- Coin Change I/II
- Longest Palindromic Substring
- Edit Distance
- Longest Increasing Subsequence
- Partition Equal Subset Sum
- Word Break
- Palindrome Partitioning
- Tiling Dominoes

### Bitmask DP
- Shortest Superstring
- Count Vowel Permutation
- Traveling Salesman Problem

### Tries
- Implement Trie
- Word Search II
- Replace Words
- Prefix and Suffix Search
- Add and Search Word (with dot wildcard)

---

## Self-Check Questions

- Do I understand how to turn a brute force recursion into a DP approach?
- Can I identify the states and transitions of any DP problem?
- Can I optimize for time and space effectively?
- Can I build and use a Trie to match prefixes and backtrack efficiently?
- Do I understand how to combine Tries with DFS for grid-based word problems?

---

## Weekly Outcome

By the end of this week, you should:
- Write correct and optimized DP solutions for 1D, 2D, tree, and bitmask problems
- Understand tradeoffs between top-down and bottom-up approaches
- Build a functional Trie and use it to solve prefix and word-search problems
- Apply both tools to hard-level interview questions with confidence