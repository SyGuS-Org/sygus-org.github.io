---
layout: page
title: SyGuS-Comp 2016
icon: medal
---

The 3<sup>rd</sup> Syntax-Guided Synthesis Competition (SyGuS-Comp)
will take place as a satellite event of CAV and SYNT 2016.

**UPDATE:**
SyGuS-Comp 2016 has concluded ([Results](#results)).
Congratulations to all winners.


### Important Dates

|------------------|------------------------------------------------------------|
| ~~30 May 2016~~  | ~~Deadline for submitting benchmarks~~                     |
| ~~14 June 2016~~ | ~~Deadline for submitting solvers and their descriptions~~ |
| ~~28 June 2016~~ | ~~Start running competition jobs on StarExec~~             |
| ~~14 July 2016~~ | ~~Notification of results to authors~~                     |
| 17 July 2016     | Solvers presentation (at SYNT'16 workshop)                 |


### Call for Participation

This is a call for participation in the 3<sup>rd</sup> Syntax-Guided Synthesis Competition
to be organized as a satellite event of SYNT and CAV 2016.

There has been a lot of recent interest in both using SyGuS solvers for various synthesis applications
and developing different solving algorithms.
The SyGuS competition (SyGuS-Comp'16) will allow solvers to compete on a large collection of benchmarks
and advance the state-of-the-art for program-synthesis tools.
We invite authors to submit their SyGuS solvers to this year's SyGuS Competition.

For questions regarding the competition please contact the organizers at <sygus-organizers@seas.upenn.edu>.


### Competition Tracks

This year's competition will have 4 tracks:
<br>
- General SyGuS track (_General_),
- Invariant synthesis track (_INV_),
- Conditional Linear Integer Arithmetic track (_CLIA_), and
- Programming By Examples track (_PBE_).

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

Nine solvers participated in SyGuS-Comp'16:
- **Alchemist-CS** (in CLIA and INV tracks) <br>
  <small><em>
    [Daniel Neider] (UIUC), Shambwaditya Saha (UIUC) and [P. Madhusudan] (UIUC)
  </em></small>
- **Alchemist-CSDT** (in CLIA track) <br>
  <small><em>
    Shambwaditya Saha (UIUC), [Daniel Neider] (UIUC) and [P. Madhusudan] (UIUC)
  </em></small>
- **CVC4 <small>1.5</small>** (in all 4 tracks) <br>
  <small><em>
    [Andrew Reynolds] (University of Iowa), [Cesare Tinelli] (University of Iowa),
    [Clark Barrett] (Stanford University), Morgan Deters (New York University)
    and Tim King (Google)
  </em></small>
- **CVC4 <small>1.5.1</small>** (in all 4 tracks) <br>
  <small><em>
    [Andrew Reynolds] (University of Iowa), [Cesare Tinelli] (University of Iowa),
    [Clark Barrett] (Stanford University) and Tim King (Google)
  </em></small>
- **Enumerative** (in General and PBE tracks) <br>
  <small><em>
    Abhishek Udupa (University of Pennsylvania)
  </em></small>
- **EUSolver** (in all 4 tracks) <br>
  <small><em>
    [Arjun Radhakrishna] (University of Pennsylvania) and Abhishek Udupa (Microsoft)
  </em></small>
- **ICE-DT** (in INV track) <br>
  <small><em>
    [Daniel Neider] (UIUC), [P. Madhusudan] (UIUC) and [Pranav Garg] (UIUC)
  </em></small>
- **Sketch-AC** (in General and PBE tracks) <br>
  <small><em>
    Jinseong Jeon (University of Maryland), [Xiaokang Qiu] (Massachusetts Institute of Technology),
    [Armando Solar-Lezama] (Massachusetts Institute of Technology) and [Jeffrey S. Foster] (University of Maryland)
  </em></small>
- **Stochastic** (in General and PBE tracks) <br>
  <small><em>
    [Mukund Raghothaman] (University of Pennsylvania)
  </em></small>


### Results

The winners for various tracks are as follows.

- **_PBE_ Track**: EUSolver
- **_INV_ Track**: ICE-DT
- **_CLIA_ Track**: CVC4
- **_General_ Track**: EUSolver

Slides for final presentation of solvers:
[ICE-DT](/assets/pdf/SyGuS-Comp'16/ICE-DT.pdf)

A detailed final report is also available [here](/assets/pdf/SyGuS-Comp'16/publication.pdf).

{% include common_links.md %}
{% include common_abbrv.md %}