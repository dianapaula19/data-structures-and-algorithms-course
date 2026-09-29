# Data Structures and Algorithms

> **Original version:** this README and some fixes were added in 2026. To see the project exactly as it was first built, browse commit [`4d07bf1`](https://github.com/dianapaula19/data-structures-and-algorithms-course/tree/4d07bf1f7cd27c8abefb13d520ac46199721c068) (2020-01-07).

Homework for the *Data Structures* course at the University of Bucharest (first year,
2019–2020), in C++. Each exercise is a small console program in its own folder (Code::Blocks
projects).

| Folder | Topics |
|---|---|
| `teme/tema_2` | Singly linked lists: an interactive menu for insertion (at the start, end, or after a value) and deletion, adding two numbers stored as lists, polynomials as linked lists |
| `teme/tema_3` | Stacks and queues on linked lists: equal numbers of a's and b's by cancelling pairs, balanced parentheses, the Josephus problem (simulation and the O(n) formula), counting islands in a matrix with DFS |
| `teme/tema_4` | Binary search trees: insertion and search, all keys between k1 and k2, and the k-th smallest key using subtree sizes |
| `teme/tema_5` | AVL trees, a max-heap, a BST of strings, and sorting: merge sort, quicksort, bitonic sort, and hybrids that switch to insertion sort on small ranges |
| `teme/tema_6` | Deque problems with file input/output |
| `bonus_seminar` | Radix sort |

## Example: k-th smallest key in a BST (`teme/tema_4/tema_4_3`)

Each node stores the size of its left subtree, so the search walks down one path:

```
$ g++ teme/tema_4/tema_4_3/main.cpp -o kth && ./kth
Numarul de elemente din arbore
7
50 30 70 20 40 60 80
20 0          <- in-order traversal: key, size of left subtree
30 1
40 0
50 3
60 0
70 1
80 0
Pozitia este:
3
50
```

## Building

Every `main.cpp` compiles on its own: `g++ -std=c++17 path/to/main.cpp -o program`.
