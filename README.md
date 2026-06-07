

## Algebraic Structures on Balance Sheet Decompositions

### 1. Net Worth as a Linear Functional (Covector)

The most precise restatement: NW is not a vector in $\mathbb{R}^2$, it's a **linear functional**

$$NW \in (\mathbb{R}^2)^* \cong \mathbb{R}^2$$

specifically $NW = (1, -1)$ acting on $(A, L)$. The balance sheet vector $\mathbf{x} = (A, L)$ lives in the primal space; NW lives in the dual. This distinction matters once you generalize, like pricing a portfolio under different probability measures corresponds to different covectors acting on the same state vector.

starting with the vector:

$$
\mathbf{x} = (A, L) \in \mathbb{R}^2, \quad A\in\mathbb{R},\quad L\in\mathbb{R}
$$

where:

- $A$ = total assets  
- $L$ = total liabilities  

then net worth becomes a linear functional on that vector space:

$$
NW(\mathbf{x}) = A - L
$$

or equivalently:

$$
NW(\mathbf{x}) =
\begin{bmatrix}
1 & -1
\end{bmatrix}
\begin{bmatrix}
A \\
L
\end{bmatrix}
$$

So net worth is essentially a projection of the 2D balance-sheet vector onto the direction $(1,-1)$.

A few neat consequences of viewing it this way:

- Two people can have identical net worths but very different balance-sheet vectors:

$$
(1M, 0) \quad\text{and}\quad (101M, 100M)
$$

Both map to:

$$
NW = 1M
$$

but the geometry/risk profile is radically different.

You can also define:

- leverage ratio:  
$$
\lambda = \frac{L}{A}
$$

- solvency region:  
$$
A \ge L
$$

- bankruptcy boundary:  
$$
A - L = 0
$$
