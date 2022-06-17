# Wick contractions for correlators of determinant and trace operators
My code for the publication https://arxiv.org/abs/2110.09458. The objective is to compute correlators in the fishnet reduction of $\mathcal{N}=4$ supersymmetric Yang-Mills theory.

## PCGG.nb
Adaptation of homonimous notebooks in https://github.com/edoardo-vescovi/wick-contractions-sym-1 and https://github.com/edoardo-vescovi/wick-contractions-sym-2 for Section 2.1.

### Initialization
Definitions: scalar and gauge progagators, vertices, PCGG, BPS-vacuum single trace, spacetime functions (propagator $I$, conformal integral $X$, functions $Y$ and $F$).
Functions: contracting array of fields freely, evaluating products of Kronecker deltas, determining topology of Feynman graph, converting arrays of scalars (with explicit $SU(N)$ matrix indices) into corresponding product of traces (hence implicit), and vice versa.

### <GG GG> tree-level
Calculate correlator of 2 determinants for Section 3.

### Save tree-level PCGG
Calculate PCGG as product of traces and saves in "PCGGDeltaAB.mx". For extra care, we include also the PCGG parts suppressed by powers $N^{-2}$ (multiplied by bookeeping variable "A") and $N^{-4}$ (by "B").
  
### <GG GG tr(...)>
Calculate correlator of 2 determinants and 1 single trace for Sections 3, 4 and Appendix B.1
  
### <GG GG tr(...)> - saved data
Data calculated by previous blocks.
  
### <tr(...) tr(...)>
Calculate correlator of 2 single traces.

## Effective theory.nb
Adaptation of homonimous notebooks in https://github.com/edoardo-vescovi/wick-contractions-sym-2 for Section 2.2. Highly optimised and commented. Results are for Sections 3, 4 and Appendix B.1.

## PCGGDeltaAB.mx
Saved data from notebook above.

## Ussyukina Davydychev.nb
Check calculation of master integrals in [82] for Appendix B.2.
