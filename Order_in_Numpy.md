### In NumPy, you can specify the memory layout of an array using these order options:

* **'C' (C-contiguous)**: Row-major order (default in NumPy, like C arrays).
* **'F' (Fortran-contiguous)**: Column-major order (like Fortran arrays).
* **'A' (Any contiguous)**: Uses 'C' order unless the array is already Fortran-contiguous.
* **'K' (Keep order)**: Preserves the order of the original array in memory.

### Order of precedence in NumPy:
* **'K'** – Keeps the existing memory order (most flexible).
* **'A'** – Follows 'F' order if already Fortran-contiguous, otherwise 'C'.
* **'C'** – Forces row-major order.
* **'F'** – Forces column-major order.

### Example:
```python
import numpy as np

arr = np.array([[1, 2], [3, 4]], order='F')  # Create in Fortran order

c_contig = np.array(arr, order='C')  # Forces C order
f_contig = np.array(arr, order='F')  # Forces F order
a_contig = np.array(arr, order='A')  # Keeps F order (since arr was F-contiguous)
k_contig = np.array(arr, order='K')  # Keeps the original memory layout (F in this case)

print(c_contig.flags['C_CONTIGUOUS'])  # True
print(f_contig.flags['F_CONTIGUOUS'])  # True
print(a_contig.flags['F_CONTIGUOUS'])  # True (keeps F)
print(k_contig.flags['F_CONTIGUOUS'])  # True (keeps original)
```
**So, 'K' > 'A' > 'C' > 'F' in terms of flexibility.**