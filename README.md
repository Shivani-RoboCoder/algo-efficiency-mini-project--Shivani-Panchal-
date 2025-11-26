# 🚀 Algorithm Efficiency Mini Project

## 📌 Project Overview
This mini-project focuses on analyzing the efficiency of different classical algorithms by measuring and comparing execution time, space usage, and overall performance. The study includes Fibonacci algorithms, multiple sorting algorithms, and Binary Search, implemented and tested using Python in a Jupyter Notebook environment.

The project helps in understanding how algorithmic complexity affects performance and how different methods behave as the size of input increases.

---

## 🏗 Task 1: Workspace Bootstrap

A private GitHub repository named **`algo-efficiency-mini-project-`** was created to store and manage the project.  
The repository includes:
- `README.md` – documentation describing the project
- `.gitignore` – excludes virtual environment, cache, logs, and checkpoints
- `Algo-efficiency-mini-project.ipynb` – main notebook running algorithms, profiling results, and graphs

### Environment Setup
A Python virtual environment was created to maintain dependency isolation. Required libraries were installed including:
- matplotlib
- numpy
- memory_profiler
- jupyter

---

## ⚙ Task 2: Algorithm Selection and Design

The following algorithms were implemented in Python:

- Fibonacci (Naïve Recursive)
- Fibonacci (Dynamic Programming)
- Merge Sort
- Quick Sort
- Insertion Sort
- Bubble Sort
- Selection Sort
- Binary Search

Each algorithm includes:
- Input and output description
- Time complexity (best, average, worst)
- Space complexity
- Suitability, usage, and trade-offs

---

## 🧠 Algorithm Details

### Fibonacci (Recursive)
Computes the nth Fibonacci number using basic recursion. Very simple but becomes extremely slow for large n due to repeated computation.
- **Time Complexity:** O(2^n)
- **Space Usage:** O(n)
- **Suitable for:** Concept demonstration only
- **Trade-off:** Not practical for large numbers

### Fibonacci (Dynamic Programming)
Computes Fibonacci efficiently using an iterative bottom-up technique.
- **Time Complexity:** O(n)
- **Space Usage:** O(1)
- **Suitable for:** Performance-heavy applications
- **Trade-off:** More complex logic than recursion

### Merge Sort
Divide-and-conquer sorting method that divides the list, sorts both halves, and merges.
- **Time Complexity:** O(n log n) best/avg/worst
- **Space Usage:** O(n)
- **Suitable for:** Large data, stable sorting
- **Trade-off:** Requires additional memory

### Quick Sort
Efficient divide-and-conquer algorithm using pivot-based partitioning.
- **Time Complexity:** O(n log n) average, O(n²) worst
- **Space Usage:** O(log n)
- **Suitable for:** Fast general sorting
- **Trade-off:** Worst-case performance when pivot is poorly chosen

### Insertion Sort
Builds sorted list one item at a time. Good for nearly sorted data.
- **Time Complexity:** O(n) best, O(n²) avg/worst
- **Space Usage:** O(1)
- **Suitable for:** Small datasets
- **Trade-off:** Very slow on large arrays

### Bubble Sort
Repeatedly swaps adjacent values if out of order.
- **Time Complexity:** O(n) best, O(n²) worst
- **Space Usage:** O(1)
- **Suitable for:** Basic learning, step-by-step understanding
- **Trade-off:** Very inefficient for real workloads

### Selection Sort
Repeatedly selects the minimum element and places it first.
- **Time Complexity:** O(n²) for all cases
- **Space Usage:** O(1)
- **Suitable for:** Low memory situations
- **Trade-off:** Always slow

### Binary Search
Searches for target value in sorted list by dividing range in half.
- **Time Complexity:** O(log n)
- **Space Usage:** O(1)
- **Suitable for:** Fast searching in sorted data
- **Trade-off:** Requires data to be sorted beforehand

---

## 📊 Performance Observation
Execution time graphs were generated using Matplotlib for:
- Fibonacci Recursive vs DP
- Sorting Algorithm Comparison

Findings:
- Fibonacci Recursive increases exponentially, becoming unusable around n = 30
- Fibonacci DP scales linearly and handles large values (n = 100000) efficiently
- Merge Sort and Quick Sort are fastest for large inputs
- Bubble Sort, Insertion Sort, Selection Sort degrade rapidly with input size

---

## 🧪 Experimental Results Summary Table

| Algorithm | Time Complexity | Space Complexity | Notes |
|-----------|----------------|------------------|--------|
| Fibonacci Recursive | O(2^n) | O(n) | Extremely slow for large n |
| Fibonacci DP | O(n) | O(1) | Best method for Fibonacc
