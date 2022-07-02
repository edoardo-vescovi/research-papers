# Gel'fand-Yaglom method for Wilson loops

My code for the publication https://arxiv.org/abs/1512.00841.
The objective is to calculate a product/ratio $Z$ of determinants of matrix-valued Laplace and Dirac operators on 2d surface embedded in $AdS_5\times S^5$ with the Gel'fand-Yaglom method in Appendix B.

## Poster
For international conference.

## Bosonic Lagrangian/
### Static gauge.nb
Basis of 10d orthogonal vectors, 2 of which tangential to surface, and projection of fluctuation vector on them.
### Nambu-Goto.nb
Expansion of string action around classical background to get Laplace operators.
### Polyakov.nb
To double check the above.
## Fermionic action/
### Spin connection.nb
Vielbein and spin connection in different coordinates.
"Poin+rect" for Poincaré coordinates in $AdS_5$ and projective coordinates in $S^5$.
"rect" for fibration coordinates in $AdS_5$ and projective coordinates in $S^5$.
"sph" for fibration coordinates in $AdS_5$ and spherical coordinates in $S^5$.
### Numerical checks.nb
Expansion of string action around classical background to get Dirac operators.

## Z/
### Z.nb
Asymptotics of Lerch function (4.6), 2d Ricci scalar (2.9) and Euler number (2.12).
Determinants of Fourier-transformed operators (3.12), (3.14), (3.16), (3.17), (3.37), (3.40)-(3.42) as function of frequency $\omega$, both for finite $\sigma_0$ and in limit $\sigma_0\to\infty$ as in (3.43)-(3.46). Identities for Lerch functions. Calculate $\log Z$: drop divergent parts as for regularisation scheme in Section 4.
### Summands.nb
Calculate $\log Z$: combine finite parts as in Sum.pdf.
### tmp.mx
Saved workspace after execution of 2 files above. Created by last line in Z.nb.
### Z sum.nb
Calculate $\log Z$: numerical sum of finite remnants over $\omega\in Z$.
### Z plot.nb
Plot of $\log Z$ and comparison with expected result in figure 1.
