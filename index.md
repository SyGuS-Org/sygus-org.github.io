---
layout: page
title: Home
---

The classical formulation of the program-synthesis problem is to find a program
that meets a correctness specification given as a logical formula.
Recent work on program synthesis and program optimization illustrates many
potential benefits of allowing the user to supplement the logical specification
with a syntactic template that constrains the space of allowed implementation.
The motivation is twofold.
First, narrowing the space of implementations makes the synthesis problem more tractable.
Second, providing a specific syntax can potentially lead to better optimizations.


### The Problem

A Syntax-Guided Synthesis problem (SyGuS, in short) is specified with respect
to a background theory $$ \mathbb{T} $$, such as Linear-Integer-Arithmetic (LIA),
that fixes the types of variables, operations on types, and their interpretation.

To synthesize a function $$ f $$ of a given type, the input consists of two constraints:
<br>
**(1)** a _semantic constraint_ given as a formula $$ \varphi $$ built from
symbols in theory $$ \mathbb{T} $$ along with $$ f $$, and
**(2)** a _syntactic constraint_ given as a (possibly infinite) set $$ \mathcal{E} $$
of expressions from $$ \mathbb{T} $$ specified by a context-free grammar.
<br>
The computational problem then is to find an implementation for the function $$ f $$,
_i.e._ an expression $$ e \in \mathcal{E} $$ such that the formula $$ \varphi[f \leftarrow e] $$ is valid.

### The Competition

The SyGuS competition (SyGuS-Comp) will allow solvers for syntax-guided synthesis
problems to compete on a large collection of benchmarks.
The motivation behind the competition is to propagate and advance research and tools on the subject.

Planning for the 6<sup>th</sup> SyGuS-Comp will commence around January 2019.
Feel free to reach us at <sygus-organizers@seas.upenn.edu> with questions and suggestions.

{% include common_links.md %}
{% include common_abbrv.md %}