## FPLP Club

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Tabling and Parsing - Alexander Vandenbroucke
> 02 May 2019

Implementing the Earley parsing algorithm using tabling in Haskell.

[Slides](slides/tabling-parsing.pdf)

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### TypeScript & Dependent Typing - Ruben Pieters
> 30 November 2018 [Slides](slides/Typescript_Dependent_Typing.pdf)

TypeScript provides a static type system on top of JavaScript. Recently TypeScript has added more and more features operating at the type level. These features enable various computations at the type level. However, the experience of the TypeScript programmer is lacking in various areas using these features. This talk explores some of the type level features and showcases some shortcomings.

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Reasoning and Derivation of Monadic Programs - Koen Pauwels
> 23 November 2018 [Slides](slides/monad-reasoning-slides.pdf)

One of the properties that sets (pure) functional programming apart from the imperative paradigm is its amenability to equational reasoning. Thanks to our ability to manage side effects in a rigorous manner with monads, we can also apply equational reasoning techniques to effectful programs.

This talk will present the functional-pearl-under-construction "Reasoning and Derivation of Monadic Programs", which aims to "develop theorems and patterns that are useful for reasoning about monadic programs". 

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Parametricity and Free Theorems - Tom Schrijvers
> 15 November 2018 [Slides](slides/parametricity.pdf)

The logical relation of System F is a very powerful property of well-typed terms
that allows us to draw many non-obvious conclusions, the so-called theorems,
by only looking at their type.

In this talk I illustrate how the logical relation can be used to derive
several free theorems.

<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Proving Haskell Coherent - Gert-Jan Bottu
> 9 November 2018 [Slides](slides/haskell_coherence_v1.pdf) Updated Slides (coming soon)

Haskell’s elaboration-based type class resolution is generally nondeterministic: 
there can be multiple ways to satisfy a wanted constraint in terms of global 
instances and locally given constraints. Coherence is the key property that keeps
this sane; it guarantees that, despite the nondeterminism, programs still behave 
predictably. Even though elaboration-based resolution is generally assumed 
coherent, this property has never formally been proven.

This talk gives a detailed introduction to Haskell's dictionary-based type class 
resolution, explains the need for a coherent elaboration and shows how we managed 
to succesfully solve this age-old problem!


<!--- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - --->
### Faster Coroutine Pipelines: A Reconstruction - Ruben Pieters
> 26 October 2018 [Slides](slides/Faster_Coroutine_Pipelines_A_Reconstruction.pdf)

Stream processing is a programming approach for efficiently handling large streams of data. It is typically used in big data applications, and is one of the reasons for its popularity. Two prominent Haskell stream processing libraries are pipes and conduit.

This presentation presents the building blocks of a simple stream processing library. Then, we look further into the details of an alternate representation for these building blocks. This alternate representation is the three-continuation approach from Spivey, which in turn is based on a very similar representation by Shivers and Might. This different representation enables an efficient definition of the merge operator. 


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

