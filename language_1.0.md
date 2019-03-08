---
layout: page
title: Specification Language (Deprecated)
icon: scroll
---

We propose a standard language for specifying syntax-guided synthesis (SyGuS) problems.
The SyGuS input format (SyGuS-IF) is closely modeled on [SMT-Lib 2].
The original proposal for SyGuS-IF can be found [here](/assets/pdf/SyGuS-IF.pdf).
This is the specification language used by the SyGuS benchmarks in the _General_ track of the SyGuS-Comp.

Here is an example SyGuS problem for a function named `max2`
that computes the maximum of two variables `x` and `y`.

```
;; The background theory is linear integer arithmetic
(set-logic LIA)

;; Name and signature of the function to be synthesize
(synth-fun max2 ((x Int) (y Int)) Int)

;; Define the grammar for allowed implementations of max2
((Start Int (x y 0 1
             (+ Start Start)
             (- Start Start)
             (ite StartBool Start Start)))
 (StartBool Bool ((and StartBool StartBool)
                  (or StartBool StartBool)
                  (not StartBool)
                  (<= Start Start)
                  (= Start Start)
                  (>= Start Start))))

(declare-var x Int)
(declare-var y Int)

;; Define the semantic constraints on the function
(constraint (>= (max2 x y) x))
(constraint (>= (max2 x y) y))
(constraint (or (= x (max2 x y)) (= y (max2 x y))))

(check-synth)
````


### Extensions

Over the years, several extensions to the original SyGuS-IF have been proposed for aiding specific synthesis scenarios.

- In 2015, we proposed the `CLIA` and `INV` extensions: [SyGuS-IF 2015](/assets/pdf/SyGuS-IF_2015.pdf)
- In 2016, we proposed the `PBE` extension: [SyGuS-IF 2016](/assets/pdf/SyGuS-IF_2016.pdf)


**UPDATE:**
We are currently in the process of drafting SyGuS-IF 2.0
which in addition to addressing several issues with the original SyGuS-IF,
also consolidates these extensions.
Stay tuned!

[SMT-Lib 2]: http://smtlib.cs.uiowa.edu/language.shtml