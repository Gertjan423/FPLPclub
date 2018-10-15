## FPLP Club

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Cochis - Klara Mar
> 12 October 2018

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

Test download button:
[Slides](slides/cochis.pdf)

Another way for downloading:
<a href="slides/cochis.pdf" download>Slides</a>


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Folds - Tom Schrijvers
> 4 October 2018

This seminar is an introduction to fold/build-fusion, deforestation and other 
recursion schemes.


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Kuifje : Quantified Information Flow with Monads in Haskell - Tom Schrijvers
> 21 October 2018

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

