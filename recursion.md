# Recursion

### Table of Contents

1. [Recursion](recursion.md)
2. [Data Abstraction](data-abstraction.md)
3. [Linked Lists](linked-lists.md)
4. [Problem Solving with Recursion](problem-solving-with-recursion.md)
5. [Stacks](stacks.md)
6. [Queues](queues.md)
7. [Algorithm Efficiency & Complexity](algorithm-efficiency-complexity.md)
8. [Sorting](sorting.md)
9. [Trees](trees.md)
10. [Tables & Priority Queues](tables-priority-queues.md)
11. [Advanced Tables & Hashing](advanced-tables-hashing.md)
12. [Graphs](graphs.md)

---

## Construction of recursive solutions:

- How can you define the problem in terms of a smaller problem of the same type?
- How does each recursive call diminish the size of the problem?
- What instance(s) of the problem can serve as the base case(s)?
- As the problem size diminishes, will you reach this base case?

## Factorial of n

Problem: Compute the factorial of an integer n

Iterative definition:

```
factorial(n) = n * (n - 1) * (n - 2) * ... * 1
    for any integer n > 0

factorial(0) = 1
```
Recurence relation:

```
factorial(n) = n * factorial(n - 1)



