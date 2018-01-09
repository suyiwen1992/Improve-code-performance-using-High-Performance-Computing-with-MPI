# Improve-code-performance-using-High-Performance-Computing
C++ program to solve the general linear system Ax=b through the following two approaches and verify that the two approaches give the same solution: (1). Call the function dgetrf() in LAPACK (http://www.netlib.org/lapack/ ) to perform the LU factorization of the coefficient matrix A and then call the function dtrsm() in LAPACK to perform the forward substitution first and then call it again to perform the backward substitution; (2). Call the mydgetrf() and mydtrsm() implemented by myself to perform the LU factorization, forward substitution, and backward substitution.

Part1mydgetrf.app shows the simple method of LU fractorization with selecting pivot in each iteration. Part2GEEP.app implements blocked the Gaussian Elimination w/ Partial Pivoting (GEPP) to solve the linear system. So, the performance can be significantly optimized by improve the cache locality.
