# Multiplicity of Limit Cycles Near Hyperbolic Polycycles of Codimension 5

<img width="803" alt="Screenshot 2024-05-31 at 00 45 03" src="https://github.com/ia-androsov/L5/assets/12882958/46c33f87-8249-4f73-8ba4-b9744bd23083">

This repository contains the Wolfram Mathematica notebooks and data files for the paper
*Multiplicity of Limit Cycles Near Hyperbolic Polycycles of Codimension 5* (I. Androsov).
The paper computes the resultant R4 of the system Q1,4 = ... = Q4,4 = 0;
the polynomial L5 is expressed through R4 (Corollary of Theorem 6.1).

- **`Poisson_L5.nb`**  
  Computation of R4 via the Poisson formula: the Gröbner basis of I4 (grevlex),
  the 6×6 matrix of multiplication by q4,4 and its determinant, R2 and R3, and
  R4 = det(m_q4,4) · R3^4. The result is written to `Res.wdx`.
  The last section checks the formulas for R2 and R3, the factorization of R4,
  the degrees and the irreducibility of the factor A (over Q and over the algebraic closure),
  and the symmetries of R4 discussed in Section 7.

- **`DiscrL5.nb`**  
  The conjecture on the discriminant: z1, z2 are eliminated from Q1 = Q2 = Q3 = 0 (z4 = 1),
  and A is shown to divide the discriminant of the eliminant with respect to z3.
  Reads `Res.wdx`.

- **`Res.wdx`**  
  The polynomial R4 in Wolfram Data Exchange format.

- **`respdf.nb`**, **`respdf.pdf`**  
  R4 written out in full.

Run `Poisson_L5.nb` first, then `DiscrL5.nb`. Both notebooks work in their own directory.
With Mathematica 14.3 on a desktop computer, `Poisson_L5.nb` takes about 15 minutes
and `DiscrL5.nb` about 2 hours.
