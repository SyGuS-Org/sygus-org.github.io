---
layout: page
title: SyGuS-Comp 2018
icon: medal
sidebar_link: true
sidebar_sort_order: 200
---

The 5<sup>th</sup> Syntax-Guided Synthesis Competition (SyGuS-Comp)
will take place as a satellite event of FLoC, CAV and SYNT 2018.

**UPDATE:**
SyGuS-Comp 2018 has concluded ([Results](#results)).
Congratulations to all winners.


### Important Dates

|------------------|---------------------------------------------------------------------------------|
| ~~1 May 2018~~   | ~~Deadline for submitting benchmarks~~                                          |
| ~~1 June 2018~~  | ~~Deadline for submitting the first version of solvers~~                        |
| ~~14 June 2018~~ | ~~Deadline for submitting the final version of solvers and their descriptions~~ |
| ~~7 July 2018~~  | ~~Notification of results to authors~~                                          |
| ~~14 July 2018~~ | ~~Awards ceremony (at FLoC Olympic games, Oxford, UK)~~                         |
| 18 July 2018     | Solvers presentation (at SYNT'18 workshop)                                      |


### Call for Participation

This is a call for participation in the 5<sup>th</sup> Syntax-Guided Synthesis Competition
to be organized as a satellite event of SYNT and CAV 2018 and as part of the FLoC Olympic games.

There has been a lot of recent interest in both using SyGuS solvers for various synthesis applications
and developing different solving algorithms.
The SyGuS competition (SyGuS-Comp'18) will allow solvers to compete on a large collection of benchmarks
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
The solver with highest score will be announced the winner of the track ---
an honor which will be accompanied by a FLoC 2018 Olympic games medal.


### Tool Submission and Description

We expect tool developers to test their solvers on the public benchmarks,
and submit the solver binaries on StarExec by the solver submission deadline.
Each solver submission should also be accompanied by a brief (1 -- 2 page in IEEE format)
description of the key ideas of the solver.


### Licensing of Tools and Benchmarks:

All benchmarks will be made public after the competition.
We encourage the tool developers to make their solvers open-source,
but participants are welcomed to submit binaries of proprietary tools as well.


### Participating Solvers

Five solvers participated in SyGuS-Comp'18:
- **CVC4** (in all 5 tracks) <br>
  <small><em>
    [Andrew Reynolds] (University of Iowa), Haniel Barbosa (University of Iowa),
    Andres Notzli (Stanford University), [Cesare Tinelli] (University of Iowa)
    and [Clark Barrett] (Stanford University)
  </em></small>
- **DryadSynth** (in INV and CLIA tracks) <br>
  <small><em>
    KangJing Huang (Purdue University), [Xiaokang Qiu] (Purdue University)
    and Yanjun Wang (Purdue University)
  </em></small>
- **EUSolver** (in all 5 tracks) <br>
  <small><em>
    [Arjun Radhakrishna] (Microsoft) and Abhishek Udupa (Microsoft)
  </em></small>
- **Horndini** (in INV track) <br>
  <small><em>
    [Deepak D'Souza] (IISc, Bangalore), P. Ezudheen (IISc, Bangalore), [P. Madhusudan] (UIUC),
    [Pranav Garg] (Amazon), [Daniel Neider] (MPI-SWS) and Shubham Ugare (IIT, Guwahati)
  </em></small>
- **LoopInvGen** (in INV track) <br>
  <small><em>
    [Saswat Padhi] (UCLA), [Rahul Sharma] (Microsoft Research, Bangalore)
    and [Todd Millstein] (UCLA)
  </em></small>


### Results

The winners for various tracks are as follows.

- **_PBE-BV_ Track**: CVC4
- **_PBE-Strings_ Track**: CVC4
- **_INV_ Track**: LoopInvGen
- **_CLIA_ Track**: CVC4 and DryadSynth
- **_General_ Track**: CVC4

Slides for final presentation of results are [here](/assets/pdf/SyGuS-Comp'18/results-slides.pdf).
<br>
Slides for final presentation of solvers:
[CVC4](/assets/pdf/SyGuS-Comp'18/CVC4.pdf),
[DryadSynth](/assets/pdf/SyGuS-Comp'18/DryadSynth.pptx),
[Horndini](/assets/pdf/SyGuS-Comp'18/Horndini.pdf),
[LoopInvGen](/assets/pdf/SyGuS-Comp'18/LoopInvGen.pdf)

[^1]: according to the pseudo-logarithmic time scale used in previous competitions
[^2]: according to the pseudo-logarithmic size scale used in previous competitions

{% include common_links.md %}
{% include common_abbrv.md %}