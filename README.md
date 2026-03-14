# java-test-0004-final-18794-ganesh
Final Project Assignment - This repository contains the complete final project code and documentation.

# Concentric Number Square Pattern in Java

## Problem

Write a Java program to print a **concentric number square pattern** using nested loops.
The pattern forms layers where the outermost layer contains the largest number and the numbers decrease as we move toward the center.

## Pattern Output

```
4 4 4 4 4 4 4
4 3 3 3 3 3 4
4 3 2 2 2 3 4
4 3 2 1 2 3 4
4 3 2 2 2 3 4
4 3 3 3 3 3 4
4 4 4 4 4 4 4
```



## Logic

1. The total size of the square is calculated as:

```
size = 2 * n - 1
```

2. For each position `(i, j)`, we calculate the minimum distance from all four edges:

* top
* bottom
* left
* right

3. The smallest distance determines which number should appear at that position.

4. The value printed is:

```
n - minimumDistance
```

This creates the layered concentric pattern.

## Time Complexity

```
O(n²)
```

Two nested loops iterate through the entire matrix.

## Space Complexity

```
O(1)
```

The program uses constant extra space since no additional data structures are stored.

