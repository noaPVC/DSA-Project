# Week 06: Hashing + Greedy + Prefix Sums

## Purpose

This week builds a toolbox of essential techniques. Hashing provides constant-time lookups and frequency tracking. Greedy methods enable local-optimum decisions with global results. Prefix sums unlock optimizations for range queries and subarray problems.

---

## Hashing (Days 1–2)

### 1. Concepts
- Hash Table: key-value mapping for O(1) average lookup time
- Python dictionaries and sets
- Handling collisions (chaining, open addressing — conceptual only)
- When hash functions matter

### 2. Common Use Cases
- Frequency counters (words, chars, numbers)
- De-duplication (e.g. detecting cycles or revisits)
- Index/value mapping (e.g. Two Sum)
- Grouping (e.g. anagrams)

### 3. Set vs Dict
- Use sets when you care only about existence/membership
- Use dicts when mapping additional data (e.g. counts, indices)

---

## Greedy Algorithms (Days 3–4)

### 1. Greedy Principle
- Locally optimal choice → globally optimal solution
- Doesn’t always work — must be proven (e.g. via greedy stays ahead or exchange arguments)

### 2. Classic Problem Types
- Activity/interval selection (earliest finish time)
- Minimum number of platforms or rooms
- Jump Game series
- Scheduling (least number of tasks, max coverage)
- Coin change with greedy constraints

### 3. Greedy with Sorting
- Often requires sorting input to apply a strategy
- Events, intervals, deadlines, profit maximization

### 4. Pitfalls
- Greedy isn’t universal — learn counterexamples
- Watch for input constraints (e.g. sorted, non-negative)

---

## Prefix Sums (Days 5–6)

### 1. Core Idea
- Build a cumulative sum array for fast subarray queries
- `prefix[i] = A[0] + ... + A[i]`
- Subarray sum from i to j: `prefix[j] - prefix[i-1]`

### 2. Variants
- 1D arrays, 2D matrices (prefix matrix)
- Difference arrays for range updates
- Rolling sums with sliding window (fixed vs dynamic)

### 3. Applications
- Find subarrays with a target sum
- Detect patterns using prefix hash maps
- Efficient range queries in large datasets

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Hash tables: frequency maps, sets, uniqueness checks |
| **2** | Hash-based problem solving: anagrams, maps, indexed tracking |
| **3** | Greedy logic: interval scheduling, jump game, greedy stays ahead |
| **4** | Greedy with sorting: task scheduling, coins, greedy failure cases |
| **5** | Prefix sums: range queries, fixed window sum, 2D prefix overview |
| **6** | Prefix sums + hashing: subarray equals k, rolling sums |
| **7** | Full synthesis review: combine hash/greedy/prefix ideas |

---

## Practice Problem Ideas

### Hashing
- Two Sum
- Group Anagrams
- Subarray Sum Equals K
- Longest Consecutive Sequence
- Top K Frequent Elements

### Greedy
- Jump Game
- Merge Intervals
- Non-overlapping Intervals
- Task Scheduler
- Gas Station

### Prefix Sum
- Subarray Sum Equals K
- Range Sum Query (Immutable)
- Find Pivot Index
- 2D Range Sum Query
- Contiguous Array (with hashmap)

---

## Self-Check Questions

- Can I use hash maps to track frequencies and indices efficiently?
- Do I recognize when a greedy solution is provably correct?
- Can I reduce O(n²) subarray sum solutions to O(n) with prefix sums?
- Do I understand when to sort to make greedy decisions viable?
- Can I identify problems that combine multiple techniques (e.g. prefix + hashmap)?

---

## Weekly Outcome

By the end of this week, you should:
- Confidently use hashing for tracking, grouping, and lookups
- Understand when and how greedy strategies apply
- Use prefix sums to solve subarray and range sum problems efficiently
- Synthesize these patterns into hybrid problem solutions