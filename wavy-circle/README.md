# Wavy Wilson loops
My code for the publication https://arxiv.org/abs/1811.09638. The input is an holomorphic function $f(z)$ on the disc. Section 2 spells the partial differential equations that define a closed curve on the plane, while Section 2.1 illustrates the perturbative method to deliver a small deformations of the circle. $ \epsilon\ll 1$ controls the the bumpiness of a wavy profile and $ \varphi\in(0,2\pi) $ spans the wavy profiles.

## Poster
For international conference.

## Sections 2-3
Analysis of generic deformation $f(z)=\epsilon e^{i\varphi} \times (\textrm{quadrinomial in } z)$ up to order $\epsilon^4$.

### Check Kruczenski's algorithm.nb
Verify equations (2.7)-(2.24).

### data.nb
Solution for curve, in 2 different parametrisations with coefficients $ b $'s and $ c $'s, in Taylor expansion up to $\epsilon^4$, to be loaded by next notebook.

### analysis.nb
Main file.
The blocks "curve" load the data on curve.
The blocks "loop" define the integrands that compute the Wilson loop at order $\lambda$ (3.1) and $\lambda^2$ (3.11).
The blocks "order" compute the Wilson loop at stated order, from $\epsilon^0 \lambda^0$ to $\epsilon^4 \lambda^2$. Here "general" use the $c$-parametrisation and "from f(z)" the $b$-parametrisation. These blocks prove the Wilson loop is independent of $\varphi$. The block "From W to logW" computes the log of Wilson loop in terms of Wilson loop; both are expansions in $\lambda$ and $\epsilon$.

### ancillary 1,2,3.nb files
Referred to in previous file.

### ancillary 5.nb
Save millions of regularised integrals for order $\lambda$ in savefile1.mx. This can be loaded by "ancillary 2.nb".

### typical integrals.nb
Recursion relations to compute regularised integrals, which compute the Wilson loop at order $\lambda$ in (3.4) and $\lambda^2$ in Appendix A.

## Section 4
Analysis of particular deformation $f(z)=\epsilon e^{i\varphi} (z^{p_1}+z^{p_2})$ up to order $\epsilon^6$.

### Check Kruczenski's algorithm.nb
Verify equations (2.1)-(2.4), construct curve, calculate Wilson loop at order $\lambda$.

### Scan p1,p2.nb
Scanning over powers and calling file above for each. It proves the Wilson loop depends on $\varphi$ beyond order $\epsilon^6$.

## Section 4 (continued)
Analysis of particular deformation $f(z)=\epsilon e^{i\varphi} \times (z^2+1)$ up to order $\epsilon^8$, not in publication.

### data.nb
Solution for curve in $b$-parametrisation, in Taylor expansion up to $\epsilon^6$, to be loaded by next notebooks.

### Check Kruczenski's algorithm.nb
Verify equations (2.1)-(2.4), construct curve, calculate Wilson loop at order $\lambda$ and $\lambda^2$.

### analysis.nb
Main file, with same structure of homonimous file above. It proves the Wilson loop depends on $\varphi$ beyond order $\epsilon^6$.
