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
