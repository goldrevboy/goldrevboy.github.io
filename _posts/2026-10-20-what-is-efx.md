---
layout: post
title: "What is EFX, and why is it still open?"
tags: [fair division]
math: true
---

*This is a sample post showing how posts work. Replace it with your own, or delete it.*

We have a set of indivisible goods $M$ and $n$ agents, each with a valuation
$v_i : 2^M \to \mathbb{R}_{\ge 0}$. An allocation $A = (A_1, \dots, A_n)$ is
**envy-free up to any good (EFX)** if for all agents $i, j$ and every good
$g \in A_j$,

$$
v_i(A_i) \;\ge\; v_i(A_j \setminus \{g\}).
$$

Envy-freeness itself can be impossible with indivisible goods: one good and
two agents already breaks it. EFX asks for the next best thing: any envy
disappears once you remove *any* single good from the envied bundle.

Whether EFX allocations always exist for additive valuations is open in
general. It is known for two agents, and for three agents with additive
valuations.

## Writing a post

1. Create a file in `_posts/` named `YYYY-MM-DD-short-title.md`.
2. Copy the front matter block from the top of this file.
3. Add `math: true` if you use LaTeX. Inline math uses `$...$`, display math uses `$$...$$`.
