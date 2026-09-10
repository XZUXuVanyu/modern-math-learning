# M002 — Subgroups (子群)

Prepared: 2026-09-10.
Delivery: begun with the learner on 2026-09-10.
Mastery: not attempted. Execution: active.
Textbook anchor: Michael Artin, Algebra, second edition, Chapter 2 §2.2, Groups and Subgroups.
This is an original lesson following the textbook topic, not a textbook excerpt.

## One objective

Determine whether a subset of a known group is itself a group under the same operation.

Prerequisites: group definition, subset notation, matrix multiplication, identity and inverse matrices. M001's review records successful matrix calculations and a repaired associativity argument; it does not establish retained mastery. This lesson uses that recorded review rather than claiming a fresh inspection of the original PDF.

## Brief recap

Associativity compares $(ab)c$ with $a(bc)$: the order stays fixed, and parentheses change.
Commutativity compares $ab$ with $ba$: the order changes.
Groups require associativity, but need not be commutative.

Your M001 group consists of the matrices $S(t)$ under multiplication. Its general product is $S(s)S(t)=S(s+t)$.

## Motivation

Once a collection of transformations is known to form a group, we often select those satisfying an additional constraint. For example, we might keep only transformations that leave a chosen vector unchanged. Does the smaller collection still form a group?

The key issue is whether composition and inversion preserve that constraint.

## Definition

Let $(G,*)$ be a group. A subset $H\subseteq G$ is a subgroup of $G$ if $H$, using the operation inherited from $G$, is itself a group. We write $H\leq G$.

"Inherited" means that for $a,b\in H$, their product is computed exactly as in $G$. We do not invent a different operation on $H$.

A subset need not be a subgroup. Membership in $G$ alone does not guarantee that products or inverses stay inside $H$.

## How to check the definition

A convenient equivalent checklist is:

1. $e_G\in H$: the identity of the parent group belongs to $H$.
2. For every $a,b\in H$, $a*b\in H$: closure under the inherited operation.
3. For every $a\in H$, its inverse $a^{-1}$ in $G$ belongs to $H$.

Why is this enough?

- Condition 1 makes $H$ nonempty and supplies its identity.
- Condition 2 makes the restricted operation a map $H\times H\to H$.
- For $a,b,c\in H$, all three are also in $G$, so $(a*b)*c=a*(b*c)$ already holds. Associativity is inherited; it does not require a fresh proof for each subgroup.
- Condition 3 supplies an inverse inside $H$, satisfying the same inverse equations.

Conversely, if $H$ is a group under the restricted operation, its identity and inverses coincide with those of $G$. To see the identity claim, choose $h\in H$ and write $e_H*h=h=e_G*h$; multiply on the right by the inverse of $h$ in $G$ and use associativity. Then $e_H=e_G$. If $b$ is the inverse of $a$ in $H$, then $a*b=e_G$, and multiplying on the left by $a^{-1}$ in $G$ gives $b=a^{-1}$.

These are consequences of the subgroup definition, not extra assumptions about a new operation.

## Worked example: even integers

Take the known group $(\mathbb Z,+)$ and its subset
$$
H=2\mathbb Z=\{2n:n\in\mathbb Z\}.
$$

1. Identity: $0=2\cdot0\in H$.
2. Closure: for arbitrary $a=2m$ and $b=2n$ in $H$,
   $$
   a+b=2(m+n)\in H
   $$
   because $m+n$ is an integer.
3. Inverses: for $a=2m\in H$, the inverse for addition is $-a=2(-m)\in H$.

Addition is associative on all integers, hence also on these integers. Therefore $2\mathbb Z\leq(\mathbb Z,+)$.

Here "inverse" means additive inverse. It does not mean the reciprocal $1/a$.

## Boundary example

The odd integers are a subset of $\mathbb Z$ but not a subgroup under addition: $1+1=2$ leaves the subset. Also, the additive identity $0$ is absent. A single failed requirement suffices.

## One homework task — original proof exercise

Let $G$ be the group of all invertible real $2\times2$ matrices under multiplication. You may take its group properties as given. Fix
$$
v=\begin{pmatrix}1\\0\end{pmatrix},
\qquad
H=\{A\in G:Av=v\}.
$$

Prove that $H$ is a subgroup of $G$.

Your argument should establish identity membership, closure, and inverse membership, and state why associativity needs no independent proof. You may use $(AB)v=A(Bv)$.

The learner owns the decisive arguments showing that the constraint $Av=v$ survives products and inverses. No solution is included. Use arbitrary matrices satisfying the condition; numerical examples alone are insufficient.

Submit the original handwriting (PNG or PDF), optionally a checked transcription, and report time spent, hints used, and the exact point of difficulty. The attempted proof and its revisions belong in the M002 conversation; do not add a separate assignment.

## Evidence and checkpoint

- M002 delivery has begun; no homework submission or learner-attempt evidence yet.
- Difficulty remains provisional; the task transfers M001's matrix work to a subset defined by a constraint.
- Existing M001 review: [homework/M001/review.md](../homework/M001/review.md).
- Next action: learner studies M002 and attempts the single subgroup proof.
- If inverse-matrix manipulation is a blocker, record it and teach the smallest prerequisite before returning to inverse membership.
