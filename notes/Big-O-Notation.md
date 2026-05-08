# Big-O Notation

## A bit of Prerequisites: Complexity Analysis & vibe-check
- Generally we use the worst-case complexity as our preferred measure of algorithm efficiency.
- Big-Oh, Big-Omega, and Big-theta are about properties of a function, not necessarily meanings.

---

## Key Idea
- We measure the run time of an algorithm by counting the number of the steps.
- Big-Oh is UPPER BOUND only, which means it can say how fast sth is but not how slow it is.
- g(n) = O(f(n)) means C * f(n) is an upper bound on g(n).
- g(n) = O(f(n)) if there are possible constants n and C such that to the right of n, the value of g(n) always lies on or below C * g(n).
- Usually used to indicate the dominating (fastest-growing) term in the function.
- O(n log n) or faster: considered efficient.

---

## Table of Important Big-O Sets
- Fastest to slowest:

| Function | Common name | Typical example |
|----------|-------------|-----------------|
| O(1) | Constant | Array access by index |
| O(log log n) | Double logarithmic | Interpolation search (well-distributed data) |
| O(log n) | Logarithmic | Binary search |
| O(√n) | Square root (sublinear) | Trial division primality check to √n |
| O(n) | Linear | One loop over n elements |
| O(n log n) | Linearithmic | Merge sort |
| O(n^2) | Quadratic | Bubble sort, naive nested loops |
| O(n^3) | Cubic | Triple loops, Floyd–Warshall shortest paths |
| O(2^n) | Exponential | Recursive brute force, Enumerating all subsets |
| O(n!) | Factorial | Brute-force TSP, all permutations |

---

## Warnings
- C has to be a constant.
- Big-Oh notation does not say what the functions are.
- Big-Oh notation does not always tell the whole story.
