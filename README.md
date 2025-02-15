# NumPy For Noobs

This provides an introduction to working with vectors and matrices using the NumPy library in Python.
As I am also a noob, I made this while also learning these things. These cover the functions which are generally used in Machine Learning.

NOTE: Not all the topics/functions mentioned are done as of now if your reading this. I will add them soon as possible.

All the best

## Notebook Contents

The notebook covers the following topics:

1. **Creating and Initializing Arrays**
  - np.array() → Create arrays from lists/tuples
  - np.zeros() → Create an array filled with zeros
  - np.ones() → Create an array filled with ones
  - np.full() → Create an array with a constant value
  - np.eye() → Identity matrix (useful in linear algebra)
  - np.linspace() → Generate evenly spaced numbers
  - np.arange() → Generate numbers with a step size
  - np.random.rand() → Random samples from uniform distribution (0,1)
  - np.random.randn() → Random samples from normal distribution
  - np.random.randint() → Random integers in a given range

2. **Data Manipulation**
  - np.reshape() → Reshape arrays (e.g., from 1D to 2D)
  - np.flatten() → Convert multi-dimensional arrays to 1D
  - np.ravel() → Flatten an array (like flatten(), but returns a view when possible)
  - np.transpose() → Transpose an array
  - np.hstack() → Horizontally stack arrays
  - np.vstack() → Vertically stack arrays
  - np.concatenate() → Concatenate multiple arrays
  - np.split() → Split an array into subarrays

3. **Indexing and Slicing**
  - np.where() → Conditional indexing (e.g., np.where(arr > 0, 1, 0))
  - np.take() → Select elements at specific indices
  - np.argsort() → Get indices that would sort an array
  - np.argmax() → Get index of max value
  - np.argmin() → Get index of min value

4. **Mathematical Operations**
  - np.add(), np.subtract(), np.multiply(), np.divide() → Element-wise operations
  - np.power() → Element-wise exponentiation
  - np.exp() → Exponential function 
  - np.log() → Natural logarithm
  - np.log10() → Base-10 logarithm
  - np.sqrt() → Square root
  - np.sin(), np.cos(), np.tan() → Trigonometric functions
  - np.dot() → Dot product (used in linear algebra)
  - np.matmul() → Matrix multiplication
  - np.linalg.inv() → Matrix inverse
  - np.linalg.det() → Determinant of a matrix
  - np.linalg.eig() → Eigenvalues and eigenvectors
  - np.linalg.svd() → Singular Value Decomposition (SVD)

5. **Statistical and Aggregation Functions**
  - np.sum() → Sum of elements
  - np.mean() → Mean of elements
  - np.median() → Median of elements
  - np.var() → Variance
  - np.std() → Standard deviation
  - np.corrcoef() → Pearson correlation coefficient
  - np.percentile() → Compute percentile of data
  - np.histogram() → Compute histogram of an array

6. **Boolean and Comparison Operations**
  - np.all() → Check if all elements satisfy a condition
  - np.any() → Check if any element satisfies a condition
  - np.isfinite() → Check for finite values
  - np.isinf() → Check for infinite values
  - np.isnan() → Check for NaNs

7. **Utility Functions for ML**
  - np.clip() → Clip values within a specified range
  - np.unique() → Find unique values in an array
  - np.bincount() → Count occurrences of values
  - np.meshgrid() → Generate coordinate grids (useful in visualization)


## Getting Started

1. Open the notebook in Google Colab.
2. Run the code cells sequentially to understand the concepts and see the output.
3. Experiment with the code by modifying values and observing the results.


## Requirements

- Python 3.x
- NumPy library

## Author

Sagar Sharma