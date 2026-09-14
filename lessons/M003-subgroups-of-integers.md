# M003 — Subgroups of the additive integers (整数加法群的子群)

Textbook: Michael Artin, Algebra, second edition, Chapter 2, Groups; topic: subgroups of the additive integers. This original lesson follows the recorded curriculum after subgroups, before cyclic groups.
Delivery: prepared for the current Lesson 3 request.
Mastery: not attempted. Execution: active.

## One objective

Classify every subgroup of $(\mathbb Z,+)$ as the set of integer multiples of one nonnegative integer.

Pacing target: 20–30 minutes study and 20–40 minutes for the single homework. M002 took 1 h learning plus 40 min of work. Keep the difficulty provisional, use explicit notation, and add no separate in-lesson assignment.

## Prerequisite recap and notation

A group is a set together with its operation. Here the parent group is $(\mathbb Z,+)$. When $H\subseteq\mathbb Z$, write its proposed group structure as
$$
(H,+|_{H\times H}).
$$
The restriction symbol means we use ordinary addition, with inputs limited to $H$. To make this a binary operation with codomain $H$, closure must be checked: $a,b\in H$ must imply $a+b\in H$. Closure in $\mathbb Z$ alone is insufficient.

The identity is $0$, and the inverse of $a$ is $-a$. Associativity is inherited once closure holds. Thus a subgroup contains $0$ and is closed under addition and negation.

For an integer $d\geq0$, define the SET
$$
d\mathbb Z=\{dk:k\in\mathbb Z\}.
$$
Its associated group uses restricted addition. In particular, $0\mathbb Z=\{0\}$.

## Motivation

Imagine allowed displacements along a line measured in integer units. Doing two allowed displacements in succession adds them; undoing one negates it. If these displacements form a subgroup, can their pattern be irregular, or must they occur at equally spaced points?

This is intuition for the question. The proof below establishes the answer for integer displacements specifically.

## Precise theorem

If $(H,+|_{H\times H})$ is a subgroup of $(\mathbb Z,+)$, there exists a unique integer $d\geq0$ such that
$$
H=d\mathbb Z.
$$
If $H\ne\{0\}$, then $d$ is the least positive element of $H$.

Conversely, for every integer $d\geq0$, the set $d\mathbb Z$ with restricted addition is a subgroup of $(\mathbb Z,+)$.

This theorem is today's one new result. We postpone cyclic-group terminology.

Two elementary integer facts are used without proof:
- Well-ordering (良序性): every nonempty set of positive integers has a least element.
- Division with remainder (带余除法): for any $h\in\mathbb Z$ and integer $d>0$, there exist integers $q,r$ with $h=qd+r$ and $0\leq r<d$. Negative $h$ are included; for example, $-7=(-2)\cdot5+3$.

## Step-by-step derivation

### 1. Check that the proposed forms work

For any $d\geq0$, $0=d\cdot0\in d\mathbb Z$. For arbitrary $dm,dn\in d\mathbb Z$,
$$
dm+dn=d(m+n)\in d\mathbb Z,
\qquad -(dm)=d(-m)\in d\mathbb Z.
$$
Associativity is inherited from integer addition. Therefore $(d\mathbb Z,+|_{d\mathbb Z\times d\mathbb Z})$ is a subgroup.

### 2. Separate the zero case

Now let $(H,+|_{H\times H})$ be an arbitrary subgroup. If $H=\{0\}$, take $d=0$.

Otherwise choose a nonzero $h\in H$. Either $h>0$, or $-h>0$ and $-h\in H$. Hence $H$ has positive elements. By well-ordering it has a least positive element; call it $d$.

### 3. Establish one inclusion

Since $d\in H$, repeated addition puts every positive integer multiple of $d$ in $H$. The identity and additive inverses supply the zero and negative multiples. Thus
$$
d\mathbb Z\subseteq H.
$$
This alone does not prove equality: $H$ might still contain other elements.

### 4. Rule out every other element

Take an arbitrary $h\in H$ and divide it by $d$:
$$
h=qd+r,\qquad 0\leq r<d.
$$
Step 3 gives $qd\in H$. Since $H$ is closed under negation and addition,
$$
r=h+(-qd)\in H.
$$
If $r>0$, it would be a positive element of $H$ smaller than $d$, contradicting the choice of $d$. Therefore $r=0$ and $h=qd\in d\mathbb Z$.

Because $h$ was arbitrary, $H\subseteq d\mathbb Z$. Combining both inclusions gives $H=d\mathbb Z$.

### 5. Check uniqueness

For $d>0$, the least positive element of $d\mathbb Z$ is exactly $d$. Hence two positive choices describing the same set must agree. The zero case is unique too: $0\mathbb Z=\{0\}$, whereas $d\mathbb Z$ contains a positive element whenever $d>0$.

## Concrete worked example

Suppose a subgroup has least positive element $4$. It contains all integer multiples of $4$ by repeated addition and inverses.

Could it also contain $14$? If so, it would contain
$$
14+(-3\cdot4)=2,
$$
contradicting the minimality of $4$.

That one calculation excludes $14$ only. To exclude EVERY nonmultiple, take arbitrary $h$ and write $h=4q+r$ with $r\in\{0,1,2,3\}$. The subgroup conditions put $r$ in $H$; minimality excludes $1,2,3$. Therefore every element is a multiple of $4$, and $H=4\mathbb Z$.

The assumption that elements are integers matters. We have not proved the same classification for subgroups of $(\mathbb R,+)$: positive real numbers need not have a least element.

## One homework task — original proof exercise

Let
$$
H=\{12m+18n:m,n\in\mathbb Z\}.
$$
Classify $(H,+|_{H\times H})$ as a subgroup of $(\mathbb Z,+)$: establish that it is a subgroup and determine the unique $d\geq0$ for which $H=d\mathbb Z$, with a proof of that equality.

Use the subgroup definition and today's theorem. A finite list of values is not a proof, and no unproved theorem about greatest common divisors is needed. This is one classification task, not a separate retention assignment.

Submit your attempt (original handwriting is welcome), study time and homework time separately, any hints used, and the exact point where you got stuck. The decisive membership arguments and value of $d$ are left to you.

## Tutor checkpoint

Basis: M002 tutor review and current progress record, not a fresh inspection of the original handwritten images.
M002 demonstrated with assistance; no conceptual blocker recorded. Its closure omission was repaired after focused hints. M003's single task checks that closure in a candidate subset is verified independently.
No M003 attempt, time report, or mastery evidence exists yet.
Next action: learner studies M003 and attempts its single classification task.
