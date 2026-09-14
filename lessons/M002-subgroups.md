# M002 — Subgroups (子群)

Prepared: 2026-09-10.
Delivery: completed with the learner on 2026-09-15.
Mastery: demonstrated with assistance. Execution: review complete.
Textbook anchor: Michael Artin, Algebra, second edition, Chapter 2 §2.2, Groups and Subgroups.
This is an original lesson following the textbook topic, not a textbook excerpt.

## One objective

Determine whether a subset of a known group is itself a group under the same operation.

Prerequisites: group definition, subset notation, matrix multiplication, identity and inverse matrices. M001's review records successful matrix calculations and a repaired associativity argument; it does not establish retained mastery.

## Brief recap

Associativity compares ((ab)c) with (a(bc)): the order stays fixed, and parentheses change.
Commutativity compares (ab) with (ba): the order changes.
Groups require associativity, but need not be commutative.

The M001 group consists of the matrices (S(t)) under multiplication, with
[
S(s)S(t)=S(s+t).
]

## Motivation

Once a collection of transformations is known to form a group, we often select those satisfying an additional constraint. The key question is whether composition and inversion preserve that constraint.

## Definition

Let ((G,*)) be a group. A subset (H\subseteq G) is a subgroup of (G) if (H), using the operation inherited from (G), is itself a group. We write (H\leq G).

“Inherited” means that for (a,b\in H), their product is computed exactly as in (G). No different operation is introduced on (H).

A subset need not be a subgroup. Membership in (G) alone does not guarantee that products or inverses stay inside (H).

## How to check the definition

A convenient equivalent checklist is:

1. (e_G\in H): the identity of the parent group belongs to (H).
2. For every (a,b\in H), (a*b\in H): closure under the inherited operation.
3. For every (a\in H), its inverse (a^{-1}) in (G) belongs to (H).

This is sufficient because:

- Condition 1 makes (H) nonempty and supplies its identity.
- Condition 2 makes the restricted operation a map (H\times H\to H).
- For (a,b,c\in H), all three lie in (G), so ((a*b)*c=a*(b*c)) is inherited from (G).
- Condition 3 supplies an inverse inside (H).

Conversely, if (H) is a group under the restricted operation, its identity and inverses coincide with those of (G). These are consequences of the subgroup definition, not assumptions about a new operation.

## Worked example: even integers

Take the known group ((\mathbb Z,+)) and
[
H=2\mathbb Z=\{2n:n\in\mathbb Z\}.
]

1. Identity: (0=2\cdot0\in H).
2. Closure: if (a=2m) and (b=2n), then
   [
   a+b=2(m+n)\in H.
   ]
3. Inverses: if (a=2m), then (-a=2(-m)\in H).

Addition is associative on all integers and hence on (H). Therefore (2\mathbb Z\leq(\mathbb Z,+)).

Here “inverse” means additive inverse, not the reciprocal (1/a).

## Boundary example

The odd integers are not a subgroup of ((\mathbb Z,+)): (1+1=2) leaves the subset, and the identity (0) is absent. One failed requirement suffices.

## One homework task — original proof exercise

Let (G) be the group of all invertible real (2\times2) matrices under multiplication. Fix
[
v=\begin{pmatrix}1\\0\end{pmatrix},
qquad
H=\{A\in G:Av=v\}.
]

Prove that (H) is a subgroup of (G), establishing identity membership, closure, inverse membership, and why associativity needs no independent proof.

The learner owns the decisive arguments. Numerical examples alone are insufficient.

## Evidence and checkpoint

- Homework submitted as two handwritten pages on 2026-09-15.
- Attempt record: [homework/M002/attempt.md](../homework/M002/attempt.md).
- Tutor review: [homework/M002/review.md](../homework/M002/review.md).
- Raw-source ledger: [homework/M002/raw/README.md](../homework/M002/raw/README.md).
- Time reported: 1 h 40 min total — 1 h learning and 40 min for an in-lesson associativity check plus the formal subgroup proof.
- Identity and inverse arguments were correct in substance.
- Original closure reasoning was missing; after a focused hint, the learner supplied a general product calculation.
- The product's lower-right entry was initially written incorrectly and then corrected to (bb') after a row-column hint.
- Associativity was correctly understood as inherited from the parent operation.
- Mastery: demonstrated with assistance.
- Execution: review complete.
- Retention: not assessed.
- Blocker: none.
- Next action: prepare the next Artin-ordered lesson. No M002 assignment remains active.
