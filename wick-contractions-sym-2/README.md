# Wick contractions for correlator of 4 determinant operators
My code for the publication https://arxiv.org/abs/2101.05117. The objective is to compute the correlator in (1) at leading and subleading order in the coupling constant $\lambda$ in $\mathcal{N}=4$ supersymmetric Yang-Mills theory.

## Notes.pdf
All calculations. Useful for reading notebooks.

## PCGG.nb
Adaptation of the homonimous notebook in https://github.com/edoardo-vescovi/wick-contractions-sym-1 for Section III.

### Initialization
Definitions: scalar and gauge progagators, vertices (scalar self-energy O, quartic-scalar vertex X, gauge exchange H), spacetime functions (propagator $I$, conformal integral $X$, functions $Y$ and $F$).
Functions: contracting array of fields (freely or inserting 1 vertex), evaluating products of Kronecker deltas and structure constants $f^{abc}$.

### Tree level
Calculate leading order with free contractions. The block "Diagram" produces (7), while "Diagram - simplest 4pt" produces (13).

### 1 loop - simplest 4pt
Calculate subleading order inserting 1 vertex. The blocks "interaction" produce (17)-(19), while the blocks "sum" produce (11)-(14).

## Effective theory
Implementation of method in Section IV.

### Initialization
Definitions: variables for integral, substitution rules, cross ratios, fermionic propagator, spacetime functions (propagator $I$, conformal integral $X$, functions $Y$ and $F$).
Functions: contracting array of fermions freely, evaluating products of Kronecker deltas.

### Derivation
Prove steps of method.

### 1-loop building blocks
Calculating (23)-(26).

### 4-pt
Check results of PCGG.nb in new method and produce figure 1.

### Simplest 4-pt
Check results of PCGG.nb in new method.
