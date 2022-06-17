# Circular Wilson loop and Bremsstrahlung function
My code for the publication https://arxiv.org/abs/1802.07726. Chapter 6 manipulates an integral in previous literature to obtain a simple expression for a Wilson loop, at any coupling constant $\lambda\in\mathbb{R}$ and winding number $n\in\mathbb{N}$.

## Derivation 1.nb
The objective is to write the real integral (6.1) in closed form (6.8). 
The notebook verifies intermediate formulas agree, within numerical accuracy and for different parameter values.
A sloppy rewriting would induce imaginary parts due to the branch-cut ambiguity of the square root.
They are weeded out through careful insertion of sign functions, whereas the final formula does not require such tweak.

## Derivation 2.nb
We derive the Wilson loop for $n=1$, the related Bremstrahlung function and their Taylor expansions at $\lambda\to\infty$.

### General identities
Definitions of many variables and integrals, with suffix M referring to Appendix A in Marino-Putrov's paper [49] and G to (3.151,3) in Gradshteyn-Ryzhik book [80].

### Limit *p &#8594; &#8734;* of Gradshteyn 3.151 3
Taylor expansion of the tabulated integral (6.10) to derive (6.8) order-by-order in powers of $1/p$.

### Translate Gradshteyn into Marino and check the latter
Establishing identities among different references' expressions.

### Check our formula for *n*-wound circle
Verifying the initial (6.1) and final formulas (6.7),(6.8) agree numerically.

### Airy function in planar limit
Limit of the Airy-function result (4.110) in [49] for $N\to \infty$. Footnote 19 comments on whether this should matches our (6.8).

### Our formula for 1-wound circle
Specialising (6.8) to winding number $n=1$ to derive (6.14) and (6.16)

### *1*-wound circle at *&lambda; &Gt; 1*
Checking the subleading order $N^{-2}$ of the Airy function is (4.124) in [49].

### Expansion *B<sub>1/2</sub>*
Taylor expansion of (6.16) for $\lambda\gg 1$

### Plot *B<sub>1/2</sub>*
Plots in figure 2.

### Generating function
An attempt to encapsulate the coefficients $V(n)$ of [49] into a generating function.
