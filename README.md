# 2D-Array-Matrices-in-C-Plus-Plus

##  Overview
A **2D array** in C++ is essentially an array of arrays, also referred to as a **matrix**. It allows storage and manipulation of tabular data in rows and columns. Matrices are widely used in mathematical computations, graphics, and data representation where elements are organized in a grid.
In C++, 2D arrays can be declared using:
```cpp
datatype arrayName[rows][columns];
```

## Common Operations on 2D Arrays

- **Matrix Addition** – Adding corresponding elements of two matrices  
- **Matrix Subtraction**  
- **Matrix Multiplication**  
- **Transpose of a Matrix** – Flipping rows and columns  
- **Finding Maximum/Minimum Element**  
- **Diagonal Sum**  

---

## Applications of 2D Arrays

- Representing mathematical matrices  
- Image processing (pixel representation)  
- Games like chess, tic-tac-toe, sudoku  
- Storing tables (e.g., marksheets, grids)  
- Dynamic programming (e.g., memoization tables)  
- Simulation of real-world grids/maps 

# 1. Matrix Input and Display in C++

## Theory

In C++, a **2D array** represents a matrix with rows and columns.  
For example, `int a1[3][3];` creates a 3x3 matrix of integers.

- Elements are accessed using two indices: `a1[i][j]` where `i` is row and `j` is column.
- Indices start from 0, so valid indices for a 3x3 matrix are 0 to 2.
- Nested loops are used to input and display matrix elements.

This program takes user input to fill the 3x3 matrix and then prints it in matrix form.

---

## Algorithm

1. Start  
2. Declare a 3x3 integer array `a1`.  
3. Use a nested loop to input elements:  
   - Outer loop runs `i` from 0 to 2 (rows)  
   - Inner loop runs `j` from 0 to 2 (columns)  
   - Input element at `a1[i][j]`  
4. Use nested loops to display the matrix elements in row-wise order.  
5. End  

---



# 2. Matrix Addition in C++

## Theory

Matrix addition involves adding corresponding elements of two matrices of the same dimensions to produce a resultant matrix.  
In C++, 2D arrays can be used to represent matrices.  
For matrix addition to be valid, both matrices must have the same number of rows and columns.

This program:
- Takes the dimensions of two matrices from the user.
- Checks if the matrices have matching dimensions.
- Inputs elements of both matrices.
- Adds the matrices element-wise.
- Displays the resultant matrix.

---

## Algorithm

1. Start  
2. Input the number of rows and columns for Matrix 1 and Matrix 2.  
3. Check if dimensions match; if not, print an error and exit.  
4. Declare three 2D arrays for Matrix 1, Matrix 2, and the Result.  
5. Input elements for Matrix 1 using nested loops.  
6. Input elements for Matrix 2 using nested loops.  
7. Add corresponding elements from Matrix 1 and Matrix 2, storing in Result.  
8. Display the Result matrix.  
9. End

# 3. Diagonal Sum of a Square Matrix in C++

## Theory

In a square matrix (where the number of rows equals the number of columns), the **main diagonal** consists of elements where the row and column indices are the same (i.e., `matrix[i][i]`).  
This program calculates the sum of the elements along the main diagonal.

Key points:
- Only square matrices have a well-defined main diagonal sum.
- The program first checks if the matrix is square.
- It inputs the elements of the matrix from the user.
- It then sums the elements where row index equals column index.
- Finally, it displays the matrix and the diagonal sum.

---

## Algorithm

1. Start  
2. Input the number of rows and columns.  
3. Check if rows and columns are equal:  
   - If not equal, print that diagonal addition is not possible and end.  
4. If equal, declare a 2D array for the matrix.  
5. Input the elements of the matrix using nested loops.  
6. Display the matrix in formatted form.  
7. Initialize `sum` to 0.  
8. Use a loop to add all elements where row index = column index (`matrix[i][i]`) to `sum`.  
9. Display the sum of the diagonal elements.  
10. End.

---

# 4. Matrix Multiplication in C++

## Theory

Matrix multiplication is the operation of multiplying two matrices to produce a third matrix.  
For two matrices **A** (size `m x n`) and **B** (size `n x p`), the resultant matrix **C** will be of size `m x p`.  
Each element `C[i][j]` is computed as the sum of the products of corresponding elements from the `i`th row of **A** and the `j`th column of **B**:

\[
C[i][j] = \sum_{k=0}^{n-1} A[i][k] \times B[k][j]
\]

Key points:
- Matrix multiplication is only possible if the number of columns in Matrix 1 equals the number of rows in Matrix 2.
- The program takes dimensions and elements for two matrices.
- It validates if multiplication is possible.
- It computes the product matrix using three nested loops.
- The resultant matrix is displayed.

---

## Algorithm

1. Start  
2. Input rows and columns for Matrix 1 (`rows1`, `cols1`).  
3. Input rows and columns for Matrix 2 (`rows2`, `cols2`).  
4. Check if `cols1 == rows2`; if not, print error and exit.  
5. Declare matrices `M1`, `M2`, and result matrix `M3`.  
6. Input elements of Matrix 1 and Matrix 2 using nested loops.  
7. Initialize all elements of `M3` to 0.  
8. Use three nested loops to compute the product matrix:  
   - Outer loop: iterate over rows of `M1`  
   - Middle loop: iterate over columns of `M2`  
   - Inner loop: perform summation of products for corresponding elements  
9. Print the resultant matrix `M3`.  
10. End.

---

# 5.Matrix Transpose in C++

## Theory

The transpose of a matrix is obtained by flipping it over its diagonal, switching the row and column indices of each element.  
If the original matrix is of size `rows x cols`, the transpose will be of size `cols x rows`.  
In the transpose matrix, the element at position `(i, j)` becomes the element at position `(j, i)`.

This program:
- Takes the dimensions and elements of a matrix from the user.
- Stores the elements in a 2D array.
- Creates a transpose matrix by swapping rows and columns.
- Displays both the original and transpose matrices.

---

## Algorithm

1. Start  
2. Input number of rows and columns.  
3. Declare a 2D array for the original matrix and another for the transpose.  
4. Input elements of the original matrix using nested loops.  
5. Display the original matrix.  
6. Create the transpose matrix by assigning `transpose[j][i] = matrix[i][j]` for all elements.  
7. Display the transpose matrix.  
8. End.

---

## Conclusion
These programs demonstrate fundamental operations on matrices using 2D arrays in C++.  
You have seen how to:
- Input and display matrices of various sizes.
- Perform key matrix operations such as addition, multiplication, transposition, and diagonal sum calculation.
- Understand the importance of validating matrix dimensions before operations to avoid errors.
- Utilize nested loops to efficiently traverse and manipulate matrix elements.
Mastering these matrix operations is essential for solving many real-world problems in fields such as computer graphics, scientific computing, engineering, and data analysis.  
They also form the foundation for more advanced topics like linear algebra libraries, image processing, and machine learning algorithms.
