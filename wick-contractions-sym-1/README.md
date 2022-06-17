# Wick contractions for correlators of determinant and trace operators
My code for the publication http://arxiv.org/abs/1906.07733. The objective is to compute correlators at leading and subleading order in the coupling constant $\lambda$ in $\mathcal{N}=4$ supersymmetric Yang-Mills theory.

## Notes files
All calculations. Useful for reading notebooks, particularly the match.

## Poster.pdf
For international conference.

## PCGG.nb
Section 4 of publication spells the partially-contracted giant gravitons (PCGG) method.

### Initialization
#### Generalities
Definitions: scalar and gauge progagators, vertices (scalar self-energy O, quartic-scalar vertex X, gauge exchange H), PCGG, single traces (BPS vacuum and made of generic scalars), spacetime functions (propagator $I$, conformal integral $X$, functions $Y$ and $F$).
Functions: contracting array of fields (freely or inserting 1 vertex), evaluating products of Kronecker deltas and structure constants $f^{abc}$, determining topology of Feynman graph.
#### Functions Y,X,F in point-splitting regularization
Definitions in the limit of one or more input points coinciding.
#### Convert lists into product of traces and vice versa
Function converting arrays of scalars (with explicit $SU(N)$ matrix indices) into corresponding product of traces (hence implicit), and vice versa.

### Miscellanea
#### Correlators of bare operators from those of renormalized ones
Relation between three-point functions of bare and renormalised operators, to understand how to extract the finite structure constant from the latter.
#### Calculate *c*
Contraction of 4 scalars using vertex X, plus that using vertex H.
#### Calculate 1-loop PCGG
Evaluating the PCGG using vertex O, plus that using vertex X, plus that using vertex H. Saves it in "diagram1and3.mx".

### <GG GG vacuum>
Correlator of 2 determinants and BPS single trace, calculated at leading order in $\lambda$. Checked subleading order equals zero.
  
### <GG GG SO(6)>
Correlator of 2 determinants and generic single trace.
  
### <vacuum vacuum SO(6)>
Correlator of 2 BPS single traces and generic single trace.
  
### <GG GG vacuum vacuum>
Correlator of 2 determinants and 2 BPS single traces. Also OPE of the result in $s$-channel limit.

## diagram1and3.mx
Created and loaded by "PCGG.nb".
  
## Integrability.nb
### p's from OPE in "PCGG"
Copy of coefficients calculated in "PCGG.nb".
### Definitions
From https://arxiv.org/pdf/1311.6404.pdf.
### Bethe equations
Solve numerically equations for SU(2) sector.
### Check pert. theory and integrability
Successful match of perturbative data calculated in "PCGG.nb" and integrability-based prediction in publication.
### Example for paper
Unused example to illustate match.
