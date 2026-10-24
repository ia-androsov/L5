# Multiplicity of Limit Cycles Near Hyperbolic Polycycles of Codimension 5

<img width="803" alt="Screenshot 2024-05-31 at 00 45 03" src="https://github.com/ia-androsov/L5/assets/12882958/46c33f87-8249-4f73-8ba4-b9744bd23083">

This repository contains the Wolfram Mathematica notebooks and data files for the paper
*Multiplicity of Limit Cycles Near Hyperbolic Polycycles of Codimension 5* (I. Androsov).
The paper computes the resultant $\mathcal{R}_4$ of the system $Q_{1,4} = \dots = Q_{4,4} = 0$;
the polynomial $\mathcal{L}_5$ is expressed through $\mathcal{R}_4$ (Corollary of Theorem 6.1).

- **`Poisson_L5.nb`**  
  Computation of $\mathcal{R}_4$ via the Poisson formula: the Gröbner basis of $I_4$ (grevlex),
  the $6 \times 6$ matrix of multiplication by $q_{4,4}$ and its determinant, $\mathcal{R}_2$ and $\mathcal{R}_3$, and

  $$\mathcal{R}_4 = \det\left(m_{q_{4,4}}\right) \cdot \mathcal{R}_3^4.$$

  The result is written to `Res.wdx`.
  The last section checks the formulas for $\mathcal{R}_2$ and $\mathcal{R}_3$, the factorization of $\mathcal{R}_4$,
  the degrees and the irreducibility of the factor $\mathfrak{A}$ (over $\mathbb{Q}$ and over the algebraic closure),
  and the symmetries of $\mathcal{R}_4$ discussed in Section 7.

- **`DiscrL5.nb`**  
  The conjecture on the discriminant: $z_1, z_2$ are eliminated from $Q_{1,4} = Q_{2,4} = Q_{3,4} = 0$ ($z_4 = 1$),
  and $\mathfrak{A}$ is shown to divide the discriminant of the eliminant with respect to $z_3$.
  Reads `Res.wdx`.

- **`Res.wdx`**  
  The polynomial $\mathcal{R}_4$ in Wolfram Data Exchange format.

- **`respdf.nb`**, **`respdf.pdf`**  
  $\mathcal{R}_4$ written out in full.

Run `Poisson_L5.nb` first, then `DiscrL5.nb`. Both notebooks work in their own directory.
With Mathematica 14.3 on a desktop computer, `Poisson_L5.nb` takes about 15 minutes
and `DiscrL5.nb` about 2 hours.
