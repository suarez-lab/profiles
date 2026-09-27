# Theses — Gabriel Suárez

**English** · [Español](README.es.md)

`Universidad Politécnica de Madrid` · `Pure mathematics` · `BSc + MSc`

Two dissertations along the same line: **Sobolev orthogonal polynomials**, approached
first through their zeros and then through the operator that generates them. Summarised
here for a reader who is not a specialist. The formal statements, the proofs and the
bibliography are in the dissertations themselves, which are not published in this
repository.

## The setting, and why it is not routine

Classical orthogonal polynomials come from an inner product that only weighs values:

```
⟨f, g⟩ = ∫ f(x) g(x) dμ(x)
```

A **Sobolev** inner product also weighs derivatives. In the *discrete* case, the
derivative terms are evaluations at finitely many points:

```
⟨f, g⟩ = ∫ f(x) g(x) dμ(x) + Σ  λ_k · f^(j_k)(c_k) · g^(j_k)(c_k)
```

That small addition removes two guarantees that the classical theory gives for free:

- **The zeros need no longer stay inside the interval of orthogonality.** They can leave
  it, and they can leave the real line. Anything built on the classical location
  argument — quadrature rules, approximation bounds — has to be re-derived rather than
  inherited.
- **Multiplication by `x`, the operator `f ↦ x·f`, need no longer be bounded.** In the
  classical case it is the well-behaved object the whole theory rests on. Here its
  boundedness is a question, and the answer depends on the points `c_k`, the orders
  `j_k` and the masses `λ_k`.

The two questions are the same question. The norm of the multiplication operator is what
confines the zeros; if the operator is unbounded, the confinement argument is gone.

## MSc thesis — the multiplication operator in discrete Sobolev spaces

A spectral and matrix analysis of that operator: **boundedness, point evaluations, zero
localisation.**

The connecting object is the **point evaluation** functional, `f ↦ f^(j)(c)`. Which of
these are bounded on the space is precisely what decides the behaviour of the operator,
and telling the bounded ones from the unbounded ones is the hard part: it is a
qualitative property of an infinite-dimensional space, not something a finite computation
reads off directly.

The contribution is an **index extending Gelfand numbers to potentially unbounded
operators**, together with the proof that **where that index stabilises identifies the
unbounded point evaluations.** Gelfand numbers are a classical way of measuring how far
a bounded operator is from being approximable by finite-rank ones; the extension carries
that measurement into a setting where the operator may not be bounded at all, and the
stabilisation point of the resulting sequence becomes a detector. A qualitative question
turns into one that a sequence of computable quantities answers.

**Computational side, in Maple.** In the polynomial basis the multiplication operator has
a **Hessenberg matrix** representation — almost triangular, one subdiagonal — and the
truncations of that matrix are what can actually be computed. Their **singular values**
are the numerical evidence: they are the finite-dimensional quantities the index is built
from, and watching them across truncations is how the stabilisation is observed rather
than merely proved.

## BSc thesis — zeros of Sobolev orthogonal polynomials

The same objects from the other end: **algorithms to compute and visualise the zero
sets**, and the connection back to **operator norms**.

Computing the zeros is a numerical problem that the loss of the classical location
guarantee makes genuinely awkward — you cannot start from "they are in the interval and
they are simple", because in general they are neither. Visualising them across families
and across the parameters of the inner product is what makes the behaviour legible: how
the zeros move as the mass `λ` grows, when they leave the interval, what happens at the
points where the derivatives are evaluated. Relating that picture back to the norm of the
multiplication operator is the bridge to the analytical work above.

## How this reads outside pure mathematics

The habit is the transferable part.

- **Stating the problem is most of the work.** "When is this operator bounded" is not the
  question you are handed; it is the question you arrive at after deciding what actually
  governs the behaviour you care about.
- **Prefer a computable criterion to a correct description.** An index whose stabilisation
  point you can observe is worth more than an exact characterisation you cannot evaluate.
- **The numerical side is evidence, not decoration.** Hessenberg truncations and their
  singular values are where a claim about an infinite-dimensional operator becomes
  something you can look at.

## Tools

Maple for the symbolic and numerical work on operators, matrix representations and
orthogonal polynomials. Python (NumPy) elsewhere.

## Full text

Not published here. Available on request — [suarez.gabriel03@gmail.com](mailto:suarez.gabriel03@gmail.com).

---

[← Profile](../gabriel.md)
