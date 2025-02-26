We use the powerful Sage function: .secondary_polytope() to generate the whole secondary polytope associated to a point-configuration 'A', and then solve a quadratic optimization problem to find the minimum GKZ vector(mGKZ).

There are two codes. 

1. mGKZ-decimal.ipynb (Jupyter Notebook file)
   Input a point-configuration 'A'.
   Output the decimal(not exact) minimal GKZ vector 'mGKZ', using Sage function minimize_constrained().
   Requirements: Sagemath-10.5 + JupyterLab

2. mGKZ-exact.ipynb + nearest-point.nb (Mathematica file)
   First, run mGKZ-exact.ipynb to generate the (in)equalities for secondary polytope, which are recorded in file (in)equations.txt (caution on the file path!). 
   Then run nearest-point.nb, it outputs the exact minimal GKZ vector. 
   Requirements: Sagemath-10.5 + JupyterLab + Mathematica-12

Limited by the algorithm of .secondary_polytope(). The number of points can not exceed 15. 
