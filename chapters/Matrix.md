<script type="text/javascript" async
    src="https://polyfill.io/v3/polyfill.min.js?features=es6">
</script>
<script type="text/javascript" async
    src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/3.2.0/es5/tex-mml-chtml.js">
</script>

# What Is a Matrix?

A **matrix** is a rectangular array of numbers, symbols, or expressions
arranged in rows and columns.

We generally write a matrix as:

$$
A = \begin{bmatrix}
a\_{11} & a\_{12} & \cdots & a\_{1n} \\
a\_{21} & a\_{22} & \cdots & a\_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a\_{m1} & a\_{m2} & \cdots & a\_{mn}
\end{bmatrix}
$$

Where:

-   *m* = number of rows  
-   *n* = number of columns  
-   *a*<sub>*i**j*</sub> = entry at row *i*, column *j*

# Types of Matrices

<table>
<colgroup>
<col style="width: 24%" />
<col style="width: 75%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Type</strong></th>
<th><strong>Definition</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Row matrix</strong></td>
<td>A matrix with only one row (size <span
class="math inline">1 × <em>n</em></span>)</td>
</tr>
<tr class="even">
<td><strong>Column matrix</strong></td>
<td>A matrix with only one column (size <span
class="math inline"><em>m</em> × 1</span>)</td>
</tr>
<tr class="odd">
<td><strong>Square matrix</strong></td>
<td>A matrix where the number of rows equals the number of columns
(<span class="math inline"><em>n</em> × <em>n</em></span>)</td>
</tr>
<tr class="even">
<td><strong>Diagonal matrix</strong></td>
<td>A square matrix where all off-diagonal elements are zero</td>
</tr>
<tr class="odd">
<td><strong>Scalar matrix</strong></td>
<td>A diagonal matrix where all diagonal elements are equal</td>
</tr>
<tr class="even">
<td><strong>Identity matrix</strong></td>
<td>A diagonal matrix where all diagonal elements are 1</td>
</tr>
<tr class="odd">
<td><strong>Zero (null) matrix</strong></td>
<td>A matrix where all elements are zero</td>
</tr>
<tr class="even">
<td><strong>Symmetric matrix</strong></td>
<td>A square matrix where <span
class="math inline"><em>A</em> = <em>A</em><sup><em>T</em></sup></span>
(equal to its transpose)</td>
</tr>
<tr class="odd">
<td><strong>Skew-symmetric matrix</strong></td>
<td>A square matrix where <span
class="math inline"><em>A</em><sup><em>T</em></sup> = −<em>A</em></span>
(transpose equals negative of itself)</td>
</tr>
<tr class="even">
<td><strong>Upper triangular matrix</strong></td>
<td>A square matrix where all elements below the main diagonal are
zero</td>
</tr>
<tr class="odd">
<td><strong>Lower triangular matrix</strong></td>
<td>A square matrix where all elements above the main diagonal are
zero</td>
</tr>
</tbody>
</table>

# Row Matrix

A **row matrix** (or row vector) is a matrix that has **only one row**
and one or more columns.

It has the general form:

$$
A = \begin{bmatrix} a\_1 & a\_2 & \cdots & a\_n \end{bmatrix}
$$

------------------------------------------------------------------------

## Definition

A matrix of size 1 × *n*, where: - 1 = number of rows  
- *n* = number of columns

------------------------------------------------------------------------

## Example

$$
R = \begin{bmatrix} 3 & 5 & 7 \end{bmatrix}
$$

Here: - Size = 1 × 3 - Elements: 3, 5, 7

------------------------------------------------------------------------

## Properties

-   It can be added or multiplied (if dimensions allow) like any matrix.
-   Its **transpose** becomes a **column matrix**:

$$
R^T = \begin{bmatrix} 3 \\ 5 \\ 7 \end{bmatrix}
$$

-   Often used to represent data points, coefficients, or vectors in a
    row form.

------------------------------------------------------------------------

# Column Matrix

A **column matrix** (or column vector) is a matrix that has **only one
column** and one or more rows.

It has the general form:

$$
A = \begin{bmatrix}
a\_1 \\
a\_2 \\
\vdots \\
a\_m
\end{bmatrix}
$$

------------------------------------------------------------------------

## Definition

A matrix of size *m* × 1, where: - *m* = number of rows  
- 1 = number of columns

------------------------------------------------------------------------

## Example

$$
C = \begin{bmatrix}
4 \\
6 \\
8
\end{bmatrix}
$$

Here: - Size = 3 × 1 - Elements: 4, 6, 8

------------------------------------------------------------------------

## Properties

-   It can be added or multiplied (if dimensions allow) like any matrix.
-   Its **transpose** becomes a **row matrix**:

$$
C^T = \begin{bmatrix} 4 & 6 & 8 \end{bmatrix}
$$

-   Commonly used to represent vectors, data series, or coefficients in
    column form.

------------------------------------------------------------------------

# Square Matrix

A **square matrix** is a matrix where the **number of rows equals the
number of columns**.

It has the general form:

$$
A = \begin{bmatrix}
a\_{11} & a\_{12} & \cdots & a\_{1n} \\
a\_{21} & a\_{22} & \cdots & a\_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a\_{n1} & a\_{n2} & \cdots & a\_{nn}
\end{bmatrix}
$$

------------------------------------------------------------------------

## Definition

A matrix of size *n* × *n*, where: - *n* = number of rows = number of
columns

------------------------------------------------------------------------

## Example

$$
S = \begin{bmatrix}
2 & 3 \\
5 & 7
\end{bmatrix}
$$

Here: - Size = 2 × 2 - Elements: 2, 3, 5, 7

Another example:

$$
S = \begin{bmatrix}
1 & 0 & 4 \\
-2 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
$$

Size = 3 × 3

------------------------------------------------------------------------

## Properties

-   Determinant is defined only for square matrices.
-   Only square matrices can have inverses (if non-singular).
-   Square matrices can be **symmetric**, **skew-symmetric**,
    **diagonal**, or **identity**.
-   The trace (sum of diagonal elements) is defined for square matrices.

------------------------------------------------------------------------

# Diagonal Matrix

A **diagonal matrix** is a square matrix where **all off-diagonal
elements are zero**, meaning only the elements on the main diagonal can
be nonzero.

It has the general form:

$$
D = \begin{bmatrix}
d\_1 & 0 & \cdots & 0 \\
0 & d\_2 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & d\_n
\end{bmatrix}
$$

------------------------------------------------------------------------

## Definition

A matrix *D* = \[*d*<sub>*i**j*</sub>\] where: -
*d*<sub>*i**j*</sub> = 0 if *i* ≠ *j* (off-diagonal entries are zero)

------------------------------------------------------------------------

## Example

$$
D = \begin{bmatrix}
3 & 0 & 0 \\
0 & -5 & 0 \\
0 & 0 & 7
\end{bmatrix}
$$

Here: - Size = 3 × 3 - Diagonal elements: 3, −5, 7

------------------------------------------------------------------------

## Properties

-   **Transpose** is itself:
    *D*<sup>*T*</sup> = *D*

-   **Inverse** (if all diagonal elements  ≠ 0) is:
    $$
    D^{-1} = \begin{bmatrix}
    1/d\_1 & 0 & \cdots & 0 \\
    0 & 1/d\_2 & \cdots & 0 \\
    \vdots & \vdots & \ddots & \vdots \\
    0 & 0 & \cdots & 1/d\_n
    \end{bmatrix}
    $$

-   **Determinant** is the product of diagonal elements:
    det (*D*) = *d*<sub>1</sub> ⋅ *d*<sub>2</sub> ⋅ … ⋅ *d*<sub>*n*</sub>

-   **Trace** is the sum of diagonal elements:
    tr(*D*) = *d*<sub>1</sub> + *d*<sub>2</sub> + … + *d*<sub>*n*</sub>

------------------------------------------------------------------------

# Scalar Matrix

A **scalar matrix** is a special type of diagonal matrix where **all
diagonal elements are equal** and **all off-diagonal elements are
zero**.

It has the general form:

$$
S = \begin{bmatrix}
k & 0 & \cdots & 0 \\
0 & k & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & k
\end{bmatrix}
$$

where *k* is a scalar (real or complex number).

------------------------------------------------------------------------

## Definition

A square matrix *S* = \[*s*<sub>*i**j*</sub>\] where: -
*s*<sub>*i**j*</sub> = 0 if *i* ≠ *j* (off-diagonal elements zero) -
*s*<sub>*i**i*</sub> = *k* (all diagonal elements equal)

------------------------------------------------------------------------

## Example

$$
S = \begin{bmatrix}
5 & 0 & 0 \\
0 & 5 & 0 \\
0 & 0 & 5
\end{bmatrix}
$$

Here: - Size = 3 × 3 - Scalar *k* = 5

------------------------------------------------------------------------

## Properties

-   Every scalar matrix is a diagonal matrix, but **not every diagonal
    matrix is scalar**.
-   It is a symmetric matrix.
-   A scalar matrix with *k* = 1 is the **identity matrix**.
-   **Inverse** (if *k* ≠ 0) is:
    $$
    S^{-1} = \frac{1}{k} I
    $$
    where *I* is the identity matrix.

------------------------------------------------------------------------

# Identity Matrix

An **identity matrix** is a special type of diagonal and scalar matrix
where **all diagonal elements are 1** and all off-diagonal elements are
zero.

It acts like the **multiplicative identity** in matrix multiplication:
*A* ⋅ *I* = *I* ⋅ *A* = *A*

------------------------------------------------------------------------

## Definition

A square matrix *I* = \[*i*<sub>*i**j*</sub>\] where: -
*i*<sub>*i**i*</sub> = 1 (diagonal elements) - *i*<sub>*i**j*</sub> = 0
if *i* ≠ *j* (off-diagonal elements)

------------------------------------------------------------------------

## Notation

$$
I\_n = \begin{bmatrix}
1 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & 1
\end{bmatrix}
$$

where *n* is the size of the matrix.

------------------------------------------------------------------------

## Example

$$
I\_3 = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

------------------------------------------------------------------------

## Properties

-   **Multiplicative identity**:
    *A* ⋅ *I* = *I* ⋅ *A* = *A*

-   **Determinant**:
    det (*I*) = 1

-   **Inverse**:
    *I*<sup>−1</sup> = *I*

-   **Transpose**:
    *I*<sup>*T*</sup> = *I*

------------------------------------------------------------------------

# Basic Matrix Operations

## ➤ Matrix Addition and Subtraction

-   Two matrices can be added or subtracted **only if** they have the
    same dimensions.
-   Element-wise operation:

*C* = *A* + *B*  where  *c*<sub>*i**j*</sub> = *a*<sub>*i**j*</sub> + *b*<sub>*i**j*</sub>

------------------------------------------------------------------------

## ➤ Scalar Multiplication

-   Multiply **every element** of the matrix by a scalar *k*:

*B* = *k**A*  where  *b*<sub>*i**j*</sub> = *k* ⋅ *a*<sub>*i**j*</sub>

------------------------------------------------------------------------

## ➤ Matrix Multiplication

-   Multiply *A*<sub>*m* × *n*</sub> by *B*<sub>*n* × *p*</sub> to get
    *C*<sub>*m* × *p*</sub>.
-   Element *c*<sub>*i**j*</sub> is the dot product of row *i* of *A*
    and column *j* of *B*:

$$
c\_{ij} = \sum\_{k=1}^{n} a\_{ik} b\_{kj}
$$

> ⚠ **Important:** Matrix multiplication is **not commutative**; that
> is, *A* ⋅ *B* ≠ *B* ⋅ *A*.

------------------------------------------------------------------------

Given two matrices:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad
B = \begin{bmatrix} 2 & 0 \\ 1 & 3 \end{bmatrix}
$$

------------------------------------------------------------------------

## Matrix Addition

Matrix addition is an **element-wise operation** where two matrices of
the **same dimensions** are added by summing their corresponding
elements.

------------------------------------------------------------------------

## Conditions

✅ Both matrices must have the **same number of rows** and **same number
of columns**.  
❌ You **cannot** add matrices of different sizes.

------------------------------------------------------------------------

## Formula

If:

$$
A = \begin{bmatrix}
a\_{11} & a\_{12} & \cdots & a\_{1n} \\
a\_{21} & a\_{22} & \cdots & a\_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a\_{m1} & a\_{m2} & \cdots & a\_{mn}
\end{bmatrix}, \quad
B = \begin{bmatrix}
b\_{11} & b\_{12} & \cdots & b\_{1n} \\
b\_{21} & b\_{22} & \cdots & b\_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
b\_{m1} & b\_{m2} & \cdots & b\_{mn}
\end{bmatrix}
$$

then:

$$
A + B = C = \begin{bmatrix}
a\_{11} + b\_{11} & a\_{12} + b\_{12} & \cdots & a\_{1n} + b\_{1n} \\
a\_{21} + b\_{21} & a\_{22} + b\_{22} & \cdots & a\_{2n} + b\_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a\_{m1} + b\_{m1} & a\_{m2} + b\_{m2} & \cdots & a\_{mn} + b\_{mn}
\end{bmatrix}
$$

------------------------------------------------------------------------

## Example

Given:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad
B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}
$$

We compute:

$$
A + B = \begin{bmatrix} 1+5 & 2+6 \\ 3+7 & 4+8 \end{bmatrix}
= \begin{bmatrix} 6 & 8 \\ 10 & 12 \end{bmatrix}
$$

------------------------------------------------------------------------

## Important Properties

-   **Commutative**:  
    *A* + *B* = *B* + *A*

-   **Associative**:  
    (*A* + *B*) + *C* = *A* + (*B* + *C*)

-   **Additive Identity** (Zero matrix):  
    *A* + 0 = *A*

------------------------------------------------------------------------

## Matrix Multiplication

Matrix multiplication is **not element-wise** — it is a **row-by-column
operation** where we multiply rows of the first matrix by columns of the
second.

------------------------------------------------------------------------

## Conditions

✅ The **number of columns** in the first matrix must equal the **number
of rows** in the second matrix.

If:

-   *A* is *m* × *n*
-   *B* is *n* × *p*

then the product:

*C* = *A* ⋅ *B*

is an *m* × *p* matrix.

------------------------------------------------------------------------

## Formula

The entry *c*<sub>*i**j*</sub> in the result matrix *C* is calculated
as:

$$
c\_{ij} = \sum\_{k=1}^{n} a\_{ik} \cdot b\_{kj}
$$

In words:  
**Take row *i* of *A*, multiply each element by the corresponding
element in column *j* of *B*, then sum them up.**

------------------------------------------------------------------------

## Example

Given:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad
B = \begin{bmatrix} 2 & 0 \\ 1 & 3 \end{bmatrix}
$$

Compute *A* ⋅ *B*:

$$
C = \begin{bmatrix}
(1 \cdot 2 + 2 \cdot 1) & (1 \cdot 0 + 2 \cdot 3) \\
(3 \cdot 2 + 4 \cdot 1) & (3 \cdot 0 + 4 \cdot 3)
\end{bmatrix}
= \begin{bmatrix} 4 & 6 \\ 10 & 12 \end{bmatrix}
$$

------------------------------------------------------------------------

## Important Properties

-   **Not commutative**:  
    *A* ⋅ *B* ≠ *B* ⋅ *A*

-   **Associative**:  
    (*A* ⋅ *B*) ⋅ *C* = *A* ⋅ (*B* ⋅ *C*)

-   **Distributive** over addition:  
    *A* ⋅ (*B* + *C*) = *A* ⋅ *B* + *A* ⋅ *C*

-   **Multiplication with identity**:  
    *A* ⋅ *I* = *A*

------------------------------------------------------------------------

## Notes

-   Multiplication with a **zero matrix** gives a zero matrix.
-   Multiplication can **change the dimensions** of the result.

------------------------------------------------------------------------

## ➤ Transpose of a Matrix

-   Flip rows and columns:

(*A*<sup>*T*</sup>)<sub>*i**j*</sub> = *A*<sub>*j**i*</sub>

# Advanced Matrix Concepts

------------------------------------------------------------------------

## ➤ Rank of a Matrix

-   The **rank** of a matrix is the maximum number of linearly
    independent rows or columns.
-   It gives the dimension of the vector space spanned by its rows or
    columns.

------------------------------------------------------------------------

## ➤ Trace of a Matrix

-   The **trace** is the sum of the diagonal elements of a square
    matrix.

$$
\text{tr}(A) = \sum\_{i=1}^{n} a\_{ii}
$$

------------------------------------------------------------------------

## ➤ Eigenvalues and Eigenvectors

Eigenvalues and eigenvectors are fundamental concepts in linear algebra,
used to understand how matrices transform space.

------------------------------------------------------------------------

## Definition

For a **square matrix** *A*, an **eigenvector** **v** and **eigenvalue**
*λ* satisfy the equation:

*A***v** = *λ***v**

This means: - *A* transforms **v** by **stretching or shrinking** it (by
*λ*) but **does not change its direction**.

------------------------------------------------------------------------

## Finding Eigenvalues

To find eigenvalues *λ*, solve the **characteristic equation**:

det (*A* − *λ**I*) = 0

where: - *I* is the identity matrix - det  is the determinant

------------------------------------------------------------------------

## Finding Eigenvectors

For each eigenvalue *λ*, solve:

(*A* − *λ**I*)**v** = 0

This gives the **nonzero solutions** **v**, which are the eigenvectors.

------------------------------------------------------------------------

## Example

Given:

$$
A = \begin{bmatrix}
2 & 1 \\
1 & 2
\end{bmatrix}
$$

### Step 1: Find eigenvalues

$$
\det(A - \lambda I) = \det \begin{bmatrix}
2 - \lambda & 1 \\
1 & 2 - \lambda
\end{bmatrix}
= (2 - \lambda)^2 - 1 = \lambda^2 - 4\lambda + 3 = 0
$$

Solve:
*λ*<sup>2</sup> − 4*λ* + 3 = 0 ⟹ (*λ* − 1)(*λ* − 3) = 0

Eigenvalues:
*λ*<sub>1</sub> = 1,  *λ*<sub>2</sub> = 3

------------------------------------------------------------------------

### Step 2: Find eigenvectors

For *λ*<sub>1</sub> = 1:

$$
(A - I) \mathbf{v} = 0 \implies \begin{bmatrix} 1 & 1 \\ 1 & 1 \end{bmatrix} \mathbf{v} = 0
$$

Solve:
*v*<sub>1</sub> + *v*<sub>2</sub> = 0 ⟹ *v*<sub>2</sub> = −*v*<sub>1</sub>

Eigenvector:
$$
\mathbf{v}\_1 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}
$$

------------------------------------------------------------------------

For *λ*<sub>2</sub> = 3:

$$
(A - 3I) \mathbf{v} = 0 \implies \begin{bmatrix} -1 & 1 \\ 1 & -1 \end{bmatrix} \mathbf{v} = 0
$$

Solve:
−*v*<sub>1</sub> + *v*<sub>2</sub> = 0 ⟹ *v*<sub>2</sub> = *v*<sub>1</sub>

Eigenvector:
$$
\mathbf{v}\_2 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

------------------------------------------------------------------------

## Properties

-   Eigenvalues can be **real or complex**.
-   The sum of eigenvalues equals the **trace** of *A*.
-   The product of eigenvalues equals the **determinant** of *A*.
-   Eigenvectors corresponding to **distinct eigenvalues** are linearly
    independent.

------------------------------------------------------------------------

## ➤ Orthogonal Matrix

-   A matrix *Q* is **orthogonal** if:

*Q*<sup>*T*</sup>*Q* = *Q**Q*<sup>*T*</sup> = *I*

This means its transpose is also its inverse.

------------------------------------------------------------------------

## ➤ Singular Matrix

-   A **singular** matrix is a square matrix with:

det (*A*) = 0

-   It is **not invertible**.

------------------------------------------------------------------------

## ➤ Positive Definite Matrix

-   A symmetric matrix *A* is **positive definite** if for all nonzero
    vectors **x**:

**x**<sup>*T*</sup>*A***x** &gt; 0

------------------------------------------------------------------------

## ➤ Diagonalization

-   A square matrix *A* is **diagonalizable** if there exists a matrix
    *P* and diagonal matrix *D* such that:

*A* = *P**D**P*<sup>−1</sup>

where *D* contains the eigenvalues and *P* contains the eigenvectors.

------------------------------------------------------------------------

## Determinant of a Matrix

The **determinant** is a special scalar value associated with a square
matrix.

It gives important information about: ✅ Whether the matrix is
invertible  
✅ Area or volume scaling under the transformation  
✅ Whether the matrix is singular (non-invertible if det = 0)

------------------------------------------------------------------------

## Conditions

✅ Determinant is **defined only** for square matrices (*n* × *n*).

------------------------------------------------------------------------

## 1️⃣ Determinant of a 2 × 2 Matrix

For:

$$
A = \begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

The determinant is:

det (*A*) = *a**d* − *b**c*

------------------------------------------------------------------------

## 2️⃣ Determinant of a 3 × 3 Matrix

For:

$$
A = \begin{bmatrix}
a\_{11} & a\_{12} & a\_{13} \\
a\_{21} & a\_{22} & a\_{23} \\
a\_{31} & a\_{32} & a\_{33}
\end{bmatrix}
$$

The determinant is:

det (*A*) = *a*<sub>11</sub>(*a*<sub>22</sub>*a*<sub>33</sub> − *a*<sub>23</sub>*a*<sub>32</sub>) − *a*<sub>12</sub>(*a*<sub>21</sub>*a*<sub>33</sub> − *a*<sub>23</sub>*a*<sub>31</sub>) + *a*<sub>13</sub>(*a*<sub>21</sub>*a*<sub>32</sub> − *a*<sub>22</sub>*a*<sub>31</sub>)

------------------------------------------------------------------------

## Example

Given:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}
$$

Compute:

det (*A*) = (1 ⋅ 4) − (2 ⋅ 3) = 4 − 6 = −2

------------------------------------------------------------------------

## Important Properties

-   **Singular matrix**:  
    If det (*A*) = 0, matrix *A* is singular (non-invertible).

-   **Multiplicative property**:  
    det (*A* ⋅ *B*) = det (*A*) ⋅ det (*B*)

-   **Determinant of transpose**:  
    det (*A*<sup>*T*</sup>) = det (*A*)

-   **Determinant of identity matrix**:  
    det (*I*) = 1

------------------------------------------------------------------------

## Notes

-   Determinants can be computed using cofactor expansion or
    row-reduction for larger matrices.
-   In R, you can use `det(A)` to compute the determinant.

------------------------------------------------------------------------

## Inverse of a Matrix

The **inverse** of a square matrix *A*, denoted *A*<sup>−1</sup>, is
another matrix such that:

*A* ⋅ *A*<sup>−1</sup> = *A*<sup>−1</sup> ⋅ *A* = *I*

where *I* is the identity matrix.

------------------------------------------------------------------------

## Conditions

✅ *A* must be a **square matrix** (*n* × *n*)  
✅ The determinant det (*A*) ≠ 0 (matrix must be **non-singular**)

If det (*A*) = 0, the matrix does **not** have an inverse.

------------------------------------------------------------------------

## 1️⃣ Inverse Formula for 2 × 2 Matrix

Given:

$$
A = \begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

The inverse is:

$$
A^{-1} = \frac{1}{\det(A)} \begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}
$$

where:

det (*A*) = *a**d* − *b**c*

------------------------------------------------------------------------

## Example

Given:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}
$$

1️⃣ Compute the determinant:

det (*A*) = (1)(4) − (2)(3) = 4 − 6 = −2

2️⃣ Apply the inverse formula:

$$
A^{-1} = \frac{1}{-2} \begin{bmatrix} 4 & -2 \\ -3 & 1 \end{bmatrix}
= \begin{bmatrix} -2 & 1 \\ 1.5 & -0.5 \end{bmatrix}
$$

------------------------------------------------------------------------

## Important Properties

-   **Multiplicative identity**:
    *A* ⋅ *A*<sup>−1</sup> = *I*

-   **Inverse of product**:
    (*A* ⋅ *B*)<sup>−1</sup> = *B*<sup>−1</sup> ⋅ *A*<sup>−1</sup>

-   **Inverse of transpose**:
    (*A*<sup>*T*</sup>)<sup>−1</sup> = (*A*<sup>−1</sup>)<sup>*T*</sup>

-   **Inverse of inverse**:
    (*A*<sup>−1</sup>)<sup>−1</sup> = *A*

------------------------------------------------------------------------

## Notes

-   For larger matrices, we usually compute the inverse using:
    -   Gaussian elimination
    -   LU decomposition
    -   In R, use the `solve(A)` function.

------------------------------------------------------------------------

## ➤ Solving Linear System *A***x** = **b**

Given:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, \quad \mathbf{b} = \begin{bmatrix} 5 \\ 11 \end{bmatrix}
$$

Solution:

**x** = *A*<sup>−1</sup>**b**

First compute:

$$
\mathbf{x} = \begin{bmatrix} -2 & 1 \\ 1.5 & -0.5 \end{bmatrix} \begin{bmatrix} 5 \\ 11 \end{bmatrix}
= \begin{bmatrix} (-2)(5) + (1)(11) \\ (1.5)(5) + (-0.5)(11) \end{bmatrix}
= \begin{bmatrix} -10 + 11 \\ 7.5 - 5.5 \end{bmatrix}
= \begin{bmatrix} 1 \\ 2 \end{bmatrix}
$$

Final solution:

*x*<sub>1</sub> = 1,  *x*<sub>2</sub> = 2
