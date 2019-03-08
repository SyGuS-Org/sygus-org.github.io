---
layout: page
title: SyGuS-Comp 2019
icon: medal
sidebar_link: true
sidebar_sort_order: 200
---

The 4<sup>th</sup> Syntax-Guided Synthesis Competition (SyGuS-Comp)
will take place as a satellite event of CAV and SYNT 2019.


### Important Dates

|------------------|---------------------------------------------------------------------------------|
| 1 May 2019       | Deadline for submitting benchmarks                                              |
| 1 June 2019      | Deadline for submitting the first version of solvers                            |
| 14 June 2019     | Deadline for submitting the final version of solvers and their descriptions     |
| 7 July 2019      | Notification of results to authors                                              |
| 13/14 July 2019  | Solvers presentation (at SYNT'19 workshop)                                      |


### Call for Participation

This is a call for participation in the 6<sup>th</sup> Syntax-Guided Synthesis Competition
to be organized as a satellite event of SYNT and CAV 2019 to be held in New York City.

There has been a lot of recent interest in both using SyGuS solvers for various synthesis applications
and developing different solving algorithms.
The SyGuS competition (SyGuS-Comp'19) will allow solvers to compete on a large collection of benchmarks
and advance the state-of-the-art for program-synthesis tools.
We invite authors to submit their SyGuS solvers to this year's SyGuS Competition.

For questions regarding the competition please contact the organizers at <sygus-organizers@seas.upenn.edu>.


### Competition Tracks

This year's competition will have 5 tracks:
<br>
- General SyGuS track (_General_),
- Invariant synthesis track (_INV_),
- Conditional Linear Integer Arithmetic track (_CLIA_),
- Programming By Examples [Strings] track (_PBE-Strings_), and
- Programming By Examples [Bit Vectors] track (_PBE-BV_).

See [Specification Language](/language.html) for more details about these tracks.


### Evaluation

Solvers will be evaluated on the [StarExec] platform,
which provided 200 dual quad-core machines with 256GB memory each.
The solvers would be run with a _TIMEOUT_ value.
The SyGuS-correctness checker, as well as the solvers from last year's competition
are available on the SyGuS community at StarExec.
Candidate participants are invited to register on StarExec,
where they can easily compare their solvers to the previous ones against the public benchmarks.


### Scoring Scheme

The scoring system is per track and as follows.
<br>
A solver that solved $$ N $$ benchmarks in the track, out of which $$ F $$ benchmarks among the fastest[^1], and
$$ S $$ benchmarks with an expression size among the smallest[^2] will receive a score: $$ 5 N + 3 F + S $$.
The solver with highest score will be announced the winner of the track.


### Tool Submission and Description

We expect tool developers to test their solvers on the public benchmarks,
and submit the solver binaries on StarExec by the solver submission deadline.
Each solver submission should also be accompanied by a brief (1 -- 2 page in IEEE format)
description of the key ideas of the solver.


### Licensing of Tools and Benchmarks:

All benchmarks will be made public after the competition.
We encourage the tool developers to make their solvers open-source,
but participants are welcomed to submit binaries of proprietary tools as well.


[^1]: according to the pseudo-logarithmic time scale used in previous competitions
[^2]: according to the pseudo-logarithmic size scale used in previous competitions

{% include common_links.md %}
{% include common_abbrv.md %}