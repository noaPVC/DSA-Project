# Week 02: Sorting & Searching

## Purpose

Sorting and searching are foundational to algorithmic thinking and optimization. This week focuses on understanding how data can be arranged for faster access and how divide-and-conquer techniques like binary search can reduce time complexity from linear to logarithmic.

---

## Sorting Algorithms (Days 1–3)

### 1. Comparison-Based Sorts
- **Bubble Sort**: pairwise swaps, rarely used but educational
- **Insertion Sort**: element-by-element insertion into sorted portion
- **Selection Sort**: selecting min element and placing it
- **Merge Sort**: divide and conquer; guaranteed O(n log n); stable
- **Quick Sort**: divide and conquer; in-place, average-case O(n log n); unstable

### 2. Non-Comparison Sorts
- **Counting Sort**: integers in limited range; linear time
- **Bucket Sort**: for uniformly distributed input
- **Radix Sort**: digit-by-digit sort, often with counting sort as subroutine

### 3. In-Place vs Stable
- Understand the difference in memory and data order preservation
- Tradeoffs in recursive stack usage vs array mutation

### 4. Python Techniques
- `sorted()`, `.sort()`, with `key` and `reverse`
- Custom sort using lambdas
- Sorting complex data structures (list of tuples/dicts)

---

## Binary Search & Variants (Days 4–5)

### 1. Standard Binary Search
- Divide the search space in half
- Efficient for sorted data
- Time complexity: O(log n)

### 2. Variants and Applications
- First/last occurrence of a value
- Lower bound, upper bound
- Find peak element
- Search in rotated sorted array
- Binary search on answer (e.g., min capacity, k-th smallest)

### 3. Pitfalls
- Infinite loops due to midpoint calculation
- Off-by-one errors
- When to return `mid`, `left`, or `right`

---

## Hybrid & Advanced Search Strategies (Day 6)

### 1. Ternary Search
- Applied in unimodal functions or hills/valleys
- Divide into three regions instead of two

### 2. Exponential Search
- Quickly find bounds, then use binary search
- Useful in unbounded/infinite arrays or file systems

### 3. Search Space Reduction
- For problems involving range or value space
- E.g., minimizing/maximizing a value under constraints

---

## Daily Breakdown

| Day | Focus Area |
|-----|------------|
| **1** | Basic sorting algorithms: selection, bubble, insertion |
| **2** | Merge sort and quicksort + comparison stability |
| **3** | Counting, radix, bucket sorts + when to use |
| **4** | Binary search: standard form and patterns |
| **5** | Binary search variations: first/last, peak, rotated arrays |
| **6** | Advanced search: binary search on answer, exponential, ternary |
| **7** | Review + strategy reflection + problem solving session |

---

## Practice Problem Ideas

### Sorting
- Sort Colors (Dutch National Flag)
- Merge Intervals
- Kth Largest Element in an Array
- Relative Sort Array
- Sort a Linked List

### Searching
- Binary Search
- Search in Rotated Sorted Array
- Find Minimum in Rotated Sorted Array
- Median of Two Sorted Arrays
- Peak Element in Array

---

## Self-Check Questions

- Can I implement both stable and unstable sorting techniques?
- Do I understand the time-space tradeoffs for each sort?
- Can I choose the right sort for the data size and type?
- Can I write binary search correctly for left-bound and right-bound queries?
- Can I apply binary search to problems beyond sorted arrays?

---

## Weekly Outcome

By the end of this week, you should:
- Be able to implement and analyze major sorting algorithms
- Use Python sorting idioms for structured data
- Confidently apply binary search and its variations
- Recognize when to apply binary search to value/range problems

