# M002 — Learner attempt

Submitted: 2026-09-15.
Status: handwritten source inspected; this record is a checked summary, not a replacement for the original pages.

## Source evidence

- Two handwritten pages were supplied in the M002 lesson conversation:
  - \`1000028358.jpg\` — source identifier \`file_00000000e9ec82098595ba32db9cd60c\`
  - \`1000028357.jpg\` — source identifier \`file_000000001fbc8206bfd8e917d5d37df1\`
- See [raw/README.md](raw/README.md) for the raw-source ledger.
- The source images remain authoritative. They were visually inspected directly; no AI-generated LaTeX transcript was used as primary evidence.

## Learner's original approach

For

$$
G=GL_2(\mathbb R),\qquad
v=\begin{pmatrix}1\\0\end{pmatrix},\qquad
H=\{A\in G:Av=v\},
$$

the learner calculated from $Av=v$ that a matrix in $H$ has the form

$$
A=\begin{pmatrix}1&a\\0&b\end{pmatrix}.
$$

The handwritten attempt then:

1. identified the identity matrix as the case $a=0,b=1$;
2. solved for an inverse candidate
   $$
   A^{-1}=\begin{pmatrix}1&-a/b\\0&1/b\end{pmatrix},
   $$
   using invertibility to obtain $b\ne0$;
3. stated that associativity is inherited from matrix multiplication on the parent group;
4. omitted an independent proof of closure, incorrectly suggesting that closure in $G$ automatically gives closure in $H$.

## Conversation revision

After the missing closure condition was identified, the learner took arbitrary

$$
A=\begin{pmatrix}1&a\\0&b\end{pmatrix},
\qquad
B=\begin{pmatrix}1&a'\\0&b'\end{pmatrix}
$$

in $H$ and attempted their product. The first response wrote the lower-right entry as $b'$. After a focused dot-product hint, the learner corrected it to $bb'$.

The completed reasoning was that the upper-right entry is real and $bb'\ne0$, so the product again has the required form and lies in $H$.

## Learner report

- Total time: 1 h 40 min.
- Learning: 1 h.
- Work described by the learner as “2 homework”: 40 min. In this repository, that consisted of one in-lesson associativity check and the one formal M002 subgroup proof.
- Hardest step: no single step identified; learner reported “not so yet.”
- Additional assistance beyond this lesson discussion: learner replied “don't need yet”; preserved here without reinterpreting it as a more specific claim.
