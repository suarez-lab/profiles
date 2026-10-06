# Theses — Gabriel Suárez

**English** · [Español](README.es.md)

Universidad Politécnica de Madrid · BSc Mathematics and Computing · MSc Advanced Mathematics

My two dissertations study Sobolev orthogonal polynomials: first their zeros,
then the multiplication operator and its matrix representation. The public
repositories below contain the mathematical sources and available computational
material. This page summarises their scope for a reader assessing my work.

## MSc thesis — multiplication operators in discrete Sobolev spaces

*Spectral and Matrix Analysis of the Multiplication Operator in Discrete Sobolev
Spaces* · **9.5/10**

**Problem.** For a polynomial inner product with discrete derivative terms,
multiplication $Dp(z)=zp(z)$ can be unbounded. The thesis studies how
finite-codimension restrictions control that failure and how it appears in
finite matrix sections.

**Mathematical work.** The manuscript studies a Gelfand-type index $Q_k(D)$,
defined as an infimum of restriction norms on polynomial subspaces of
codimension at most $k$, allowing the value $+\infty$. This is the
restriction-based viewpoint of Gelfand numbers.

For the configuration of normalized circle measure of radius $R$ and $N$
distinct first-derivative atoms with unit weights, let $m$ count the atoms on or
outside the circle. The manuscript establishes:

- $Q_k(D)=+\infty$ for $0\le k<m$;
- $Q_k(D)$ is finite for $m\le k<N$;
- $Q_k(D)=R$ for $k\ge N$.

The first finite index is therefore $Q_m(D)$. This statement is about the
specified configuration; it is not a universal detector for arbitrary Sobolev
inner products. The distinction between first finiteness and eventual equality
to $R$ matters.

**Computational work.** Maple routines investigate finite Hessenberg
representations and their singular values. Eigenvalues of principal sections
give the corresponding orthogonal-polynomial zeros; the manuscript relates
limits of ordered singular values to $Q_k(D)$. Finite computations illustrate
these results and do not prove an asymptotic statement by themselves.

**Public evidence.** [Repository and overview](https://github.com/Gabotelli/sobolev-multiplication-operators) ·
[Main manuscript source](https://github.com/Gabotelli/sobolev-multiplication-operators/blob/master/Plantilla%20TFM/main.tex) ·
[Circle-measure results](https://github.com/Gabotelli/sobolev-multiplication-operators/blob/master/Plantilla%20TFM/chapters/capitulo3-estabilizacion.tex) ·
[Defense source](https://github.com/Gabotelli/sobolev-multiplication-operators/blob/master/Plantilla%20TFM/presentacion/defensa.tex).

**Reproduction status.** Standalone Maple worksheets are not currently included.
The repository contains LaTeX sources and existing figures; a clean manuscript
and slide build has not been verified.

## BSc thesis — zeros of Sobolev orthogonal polynomials

*Zeros of Sobolev Orthogonal Polynomials: Visualization and Analysis* · **9.4/10**

**Problem.** Adding derivative terms changes classical zero-localisation
arguments. The work investigates zero configurations and their relationship to
multiplication-operator norms.

**Computational contribution.** Maple algorithms construct polynomial families,
compute and visualise their zeros, and compare zero localisation with operator
norms and singular values. Experiments include real and complex support
configurations and support the formulation and investigation of conjectures.
The manuscript distinguishes numerical observations from proven results.

**Public evidence.** [Repository and overview](https://github.com/Gabotelli/sobolev-orthogonal-polynomials) ·
[Maple worksheet](https://github.com/Gabotelli/sobolev-orthogonal-polynomials/blob/main/maple/tfg7.mw) ·
[Main manuscript source](https://github.com/Gabotelli/sobolev-orthogonal-polynomials/blob/main/latex/tfg_latex_etsiinf-2023.02.20/tfg_etsiinf_plantilla.tex) ·
[Maple inventory](https://github.com/Gabotelli/sobolev-orthogonal-polynomials/blob/main/docs/maple-inventory.md).

**Reproduction status.** Four `.mw` worksheets and a `.maple` workbook are
available. The remaining 55 `.m` files are serialized states, not independent
programs. Some worksheets depend on saved states or external reads; a portable
regeneration of every experiment and figure has not been verified.

## Authorship and tools

This work is connected to `EGS26`, an article not yet published, prepared jointly with my thesis supervisors, Carmen Escribano and Raquel Gonzalo. Work associated with that article is collaborative; this page does not attribute all of its results to me alone.

The theses are my academic work. Cited research, university templates and
included routines retain their respective attribution; this summary does not
claim that every result or routine is original. Maple is used for the thesis
computations, and LaTeX for the manuscripts and defense material.

Compiled PDFs are not currently included in these repositories. For enquiries:
[suarez.gabriel03@gmail.com](mailto:suarez.gabriel03@gmail.com).

---

[← Profile](../gabriel.md)
