---
layout: page
title: SyGuS-Comp 2017
icon: medal
---

The 4<sup>th</sup> Syntax-Guided Synthesis Competition (SyGuS-Comp)
will take place as a satellite event of CAV and SYNT 2017.

**UPDATE:**
SyGuS-Comp 2017 has concluded ([Results](#results)).
Congratulations to all winners.


### Important Dates

|------------------|---------------------------------------------------------------------------------|
| ~~15 May 2017~~  | ~~Deadline for submitting benchmarks~~                                          |
| ~~7 June 2017~~  | ~~Deadline for submitting the first version of solvers~~                        |
| ~~14 June 2017~~ | ~~Deadline for submitting the final version of solvers and their descriptions~~ |
| ~~14 July 2017~~ | ~~Notification of results to authors~~                                          |
| 22 July 2017     | Solvers presentation (at SYNT'17 workshop)                                      |


### Call for Participation

This is a call for participation in the 4<sup>th</sup> Syntax-Guided Synthesis Competition
to be organized as a satellite event of SYNT and CAV 2017.

There has been a lot of recent interest in both using SyGuS solvers for various synthesis applications
and developing different solving algorithms.
The SyGuS competition (SyGuS-Comp'17) will allow solvers to compete on a large collection of benchmarks
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

Five solvers participated in SyGuS-Comp'17:
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
- **Euphony** (in all 5 tracks) <br>
  <small><em>
    [Woosuk Lee] (University of Pennsylvania), [Arjun Radhakrishna] (Microsoft) and Abhishek Udupa (Microsoft)
  </em></small>
- **E3Solver** (in PBE-BV track) <br>
  <small><em>
    Ammar Ben Khadra (University of Kaiserslautern)
  </em></small>
- **LoopInvGen** (in INV track) <br>
  <small><em>
    [Saswat Padhi] (UCLA) and [Todd Millstein] (UCLA)
  </em></small>


### Results

The winners for various tracks are as follows.

- **_PBE-BV_ Track**: E3Solver
- **_PBE-Strings_ Track**: CVC4
- **_INV_ Track**: LoopInvGen
- **_CLIA_ Track**: CVC4
- **_General_ Track**: CVC4

Slides for final presentation of results are [here](/assets/pdf/SyGuS-Comp'17/results-slides.pdf).
<br>
Slides for final presentation of solvers:
[CVC4](/assets/pdf/SyGuS-Comp'17/CVC4.pdf),
[DryadSynth](/assets/pdf/SyGuS-Comp'17/DryadSynth.pptx),
[E3Solver](/assets/pdf/SyGuS-Comp'17/E3Solver.pdf),
[LoopInvGen](/assets/pdf/SyGuS-Comp'17/LoopInvGen.pdf)

A detailed final report is also available [here](/assets/pdf/SyGuS-Comp'17/publication.pdf).

{% include common_links.md %}
{% include common_abbrv.md %}