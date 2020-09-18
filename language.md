---
layout: page
title: Specification Language
icon: scroll

sidebar_link: true
sidebar_sort_order: 100
---

We propose a standard language for specifying syntax-guided synthesis (SyGuS) problems.
The SyGuS input format (SyGuS-IF) is closely modeled on [SMT-Lib 2].

<i class='fas fa-fw fa-file-pdf'></i>
[The SyGuS Language Standard Version 2.0](/assets/pdf/SyGuS-IF_2.0.pdf)

Here is an example SyGuS problem for a function named `max2`
that computes the maximum of two variables `x` and `y`.

```
;; The background theory is linear integer arithmetic
(set-logic LIA)

;; Name and signature of the function to be synthesized
(synth-fun max2 ((x Int) (y Int)) Int
    
    ;; Declare the non-terminals that would be used in the grammar
    ((I Int) (B Bool))

    ;; Define the grammar for allowed implementations of max2
    ((I Int (x y 0 1
             (+ I I) (- I I)
             (ite B I I)))
     (B Bool ((and B B) (or B B) (not B)
              (= I I) (<= I I) (>= I I))))
)

(declare-var x Int)
(declare-var y Int)

;; Define the semantic constraints on the function
(constraint (>= (max2 x y) x))
(constraint (>= (max2 x y) y))
(constraint (or (= x (max2 x y)) (= y (max2 x y))))

(check-synth)
````

Our initial proposal for SyGuS-IF (ver. 1.0) and its extensions can be found [here](/language_1.0).
However, this original proposal is now deprecated.
We revised our input format in 2019 and proposed SyGuS-IF ver. 2.0,
which is more compliant with SMT-LIB version 2.6,
includes minor changes to the concrete syntax for commands,
and eliminates several deprecated features of the previous format.

[SMT-Lib 2]: http://smtlib.cs.uiowa.edu/language.shtml