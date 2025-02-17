## C-like vs. Fortran-like Index Ordering

When reshaping or flattening an array in NumPy, we can use two main memory orders:

1. **C-like order (`order='C'`)** → Row-major ordering.
2. **Fortran-like order (`order='F'`)** → Column-major ordering.

These determine how the elements are stored and read in memory.

---

### C-like (Row-Major) Ordering (`order='C'`)

- This follows the **row-first** principle.
- Elements are stored **row by row** in memory (left to right).

#### Example:
```python
import numpy as np

a = np.array([0, 1, 2, 3, 4, 5])  # Original 1D array

# Reshape into (2, 3) using C-like order
b = np.reshape(a, (2, 3), order='C')
print(b)
```

#### Output:
```python
[[0 1 2]  
 [3 4 5]]
```
#### How the elements are stored in memory:
`0  1  2  3  4  5  → (Stored row-wise)`

- First row [0, 1, 2], then second row [3, 4, 5].

---

### Fortran-like (Column-Major) Ordering (`order='F'`)

- This follows the column-first principle.
- Elements are stored column by column in memory.

#### Example:
```python
b = np.reshape(a, (2, 3), order='F')
print(b)
```
#### Output:
```python
[[0 4 3]  
 [2 1 5]]
 ```
#### How the elements are stored in memory:
`0  2  4  1  3  5  → (Stored column-wise)`
- First column [0, 2], second column [4, 1], third column [3, 5].
---