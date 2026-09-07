# M001 — Definition of a group (群)

Delivered: 2026-09-07. Mastery: not attempted. Execution: active.
Textbook anchor: Artin, Algebra, second edition, Chapter 2, especially §2.2. This is an original short lesson following that topic, not a textbook excerpt.

## One objective and prerequisites

Understand and check the definition of a group. Recall ordinary integer addition and matrix multiplication. The latter is assumed provisionally for the homework; report if it is unfamiliar.

## Motivation

In physics we often combine transformations: perform one rotation, then another. We can do nothing or undo a transformation. Group theory abstracts the algebraic structure of such reversible operations. This motivates the definition; it is not a proof about every physical transformation.

## Definition

A group consists of a nonempty set $G$ and a specified operation $*$ with these properties:

1. Closure: every $a,b\in G$ gives one well-defined result $a*b\in G$.
2. Associativity: $(a*b)*c=a*(b*c)$ for all $a,b,c\in G$.
3. Identity: there is $e\in G$ such that $e*a=a*e=a$ for every $a\in G$.
4. Inverses: for each $a\in G$, there is $b\in G$ such that $a*b=b*a=e$.

Equivalently, specifying the operation as a map $G\times G\to G$ already includes well-definedness and closure; the other three conditions are the group axioms. The four-condition checklist here makes closure explicit.

$*$ can mean addition, matrix multiplication, or transformation composition. Associativity concerns parentheses. It does not assert $a*b=b*a$.

## Worked example: integers under addition

Check $(\mathbb Z,+)$ step by step:

1. The sum of two integers is an integer: closure.
2. Ordinary addition satisfies $(a+b)+c=a+(b+c)$: associativity.
3. $0+a=a+0=a$, so $0$ is an identity.
4. For each integer $a$, the integer $-a$ satisfies $a+(-a)=(-a)+a=0$.

Thus $(\mathbb Z,+)$ is a group. This verifies the definition using known properties of integer arithmetic.

The operation matters. $(\mathbb Z,\times)$ is not a group: $2$ has no multiplicative inverse in the integers.

## One homework task — original proof exercise

Let

$$
S(t)=\begin{pmatrix}1&t\\0&1\end{pmatrix},\qquad
G=\{S(t):t\in\mathbb R\}.
$$

Prove that $G$ is a group under matrix multiplication, explicitly checking all four conditions. You may use the known associativity of matrix multiplication.

Starting hint: compute $S(s)S(t)$ for arbitrary real $s,t$. A few numerical examples cannot establish closure for every pair.

The learner owns the general product calculation, identity/inverse reasoning, and complete argument. No solution is stored in this repository.

Submit original handwriting and optionally a checked transcription; report time spent and where you got stuck in [the attempt record](../homework/M001/attempt.md).

## Checkpoint

No attempt received. Tutor review and learner explanation remain pending. If a prerequisite is missing, record it in progress.md and return to the same proof after a bounded prerequisite lesson.
