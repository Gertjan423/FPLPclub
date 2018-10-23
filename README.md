## FPLP Club

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Pipes and Orthogonal Scott-Encodings - Ruben Pieters
> 26 October 2018

Ruben talks about his paper on pipes and orthogonal Scott-encodings.


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Domain Theory - Alexander Vandenbroucke
> 19 October 2018 : [Slides](slides/domain_theory.pdf)

There are different approaches to assigning meaning or semantics to programming
languages. This talk focusses on the denotational style of semantics, whereby
we directly assign meaning to a program by mapping its syntax to mathematical
objects, its denotation. By reasoning about the denotations of programs, we
reason about the programs themselves. Domain theory concerns itself with
finding "good" collections of mathematical objects.

To illustrate this, the talk studies the lattice-based domain for the untyped
lambda calculus, as explored by Dana Scott in his seminal paper (Continuous
Lattices, Dana Scott, 1972).


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Cochis - Klara Mar
> 12 October 2018 : [Slides](slides/cochis.pdf)

Implicit Progamming (IP) mechanisms infer values by type-directed resolution, 
making programs more compact and easier to read. Examples of IP mechanisms include 
Haskell’s type classes, Scala’s implicits, Agda’s instance arguments, Coq’s type 
classes, and Rust’s traits. The design of IP mechanisms has led to heated debate:
proponents of one school argue for the desirability of strong reasoning properties;
while proponents of another school argue for the power and flexibility of local 
scoping or overlapping instances. The current state of affairs seems to indicate 
that the two goals are at odds with one another and cannot easily be reconciled.

This talk presents COCHIS, the Calculus Of CoHerent ImplicitS, an improved variant
of the implicit calculus that offers flexibility while preserving two key properties:
coherence and stability of substitutions. COCHIS supports polymorphism, local 
scoping, overlapping instances, first-class instances, and higher-order rules, 
while remaining type safe, coherent and stable under substitution.


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Folds - Tom Schrijvers
> 4 October 2018 : [Slides1](slides/universe_of_types.pdf), [Slides2](slides/bringing_functions_into_the_fold)

This seminar is an introduction to datatype generic programming and structural recursion.


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Kuifje : Quantified Information Flow with Monads in Haskell - Tom Schrijvers
> 21 September 2018 : [Slides](slides/qif.pdf)

Programs that manipulate private information must usually release part of
their secret to achieve anything useful. Yet, unintended leaks, which could
be avoided by more careful programming, are a major concern. Quantifying
the information that does flow has been proposed as a means to analyse the
severity and impact of such leaks.

This talk presents Kuifje, a domain-specific language (DSL) for
Quantitative Information Flow (QIF) in Haskell. Kuifje implements the
recent insight that a monadic semantics based on hyper-distributions
(distributions of distributions) generalises earlier QIF approaches based
on Shannon entropy for channels to different notions of entropy for
programs.

The talk develops Kuifje in a gentle fashion, starting from a simple
denotational semantics for a small imperative language. This development
not only benefits from Haskell’s support for monads and DSLs, but also puts
two elementary functional programming patterns, monoids and folds, to good
use. The result is an efficient implementation of the hyper-distribution
semantics that runs interesting example scenarios.

This is talk is based on joint work with Carroll Morgan, Annabelle McIver
and Jeremy Gibbons.

