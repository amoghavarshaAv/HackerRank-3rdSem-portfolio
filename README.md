# HackerRank 3rd-Semester CSE Problem-Solving Portfolio

## Repository Overview
This repository contains optimal algorithmic solutions for the 5 mandatory HackerRank studio problems required for the 3rd-semester Computer Science & Engineering curriculum. Every solution is implemented with a focus on optimal Time and Space Complexity.

* **HackerRank Profile:** [Your Profile Link Here](https://www.hackerrank.com/your_username)
* **Earned Badge:** 3-Star Problem Solving / Language Badge

---

## Complexity Summary Table

| No. | Problem Name | Domain / Topic | Time Complexity | Space Complexity | Status |
|---|---|---|---|---|---|
| 1 | Diagonal Difference | 2D Arrays / Matrices | $O(N)$ | $O(1)$ | Accepted |
| 2 | Dynamic Array | Data Structures / Vectors | $O(N + Q)$ | $O(N)$ | Accepted |
| 3 | Time Conversion | Strings & Parsing | $O(1)$ | $O(1)$ | Accepted |
| 4 | Compare the Triplets | Arrays & Logic | $O(1)$ | $O(1)$ | Accepted |
| 5 | Sparse Arrays | Hash Maps / Strings | $O(N + Q)$ | $O(N)$ | Accepted |

---

## Problem Approaches & Key Concepts

### 1. Diagonal Difference
* **Approach:** A single loop runs $N$ times. In iteration $i$, `matrix[i][i]` (primary diagonal) and `matrix[i][N - 1 - i]` (secondary diagonal) are accumulated simultaneously.
* **Optimization:** Avoids nested loops ($O(N^2)$), keeping the runtime strictly linear $O(N)$ with auxiliary space $O(1)$.

### 2. Dynamic Array
* **Approach:** Uses a dynamically allocated 2D sequence (`vector<vector<int>>` or `ArrayList<List<Integer>>`) combined with bitwise XOR indexing: `idx = (x ^ lastAnswer) % n`.
* **Optimization:** Modulo indexing prevents out-of-bounds access while dynamic resizing ensures minimum memory overhead.

### 3. Time Conversion
* **Approach:** Direct string parsing extracts the AM/PM designation, hour, and minute components. Hours are converted using modulo arithmetic rules before reformatting into 24-hour military format.
* **Optimization:** Operates in constant $O(1)$ time and space since input strings are fixed length (10 characters).

### 4. Compare the Triplets
* **Approach:** Performs direct element-wise comparison between two 3-element arrays in a single pass while tracking score states.
* **Optimization:** Runs in fixed time $O(1)$ and uses minimal memory allocations $O(1)$.

### 5. Sparse Arrays
* **Approach:** Uses a Hash Map (Unordered Map / Counter) to perform a frequency count on input strings in $O(N)$ time. Queries are answered in $O(1)$ average time lookup.
* **Optimization:** Reduces overall computational complexity from brute force $O(N \times Q)$ down to optimal $O(N + Q)$.

---

## Submission Verification & Badges
* Screenshots showing full test-case passage for each problem can be found in their respective problem subfolders.
* Verification evidence for the HackerRank badge is documented in the submission report.
