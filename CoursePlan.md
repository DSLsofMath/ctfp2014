# Category Theory and Functional Programming

* 7.5hp, Hybrid course (shared between MSc and PhD level), Autumn 2014
* Examiner: Patrik Jansson
* Lecturer: Cezar Ionescu

----

## Course Description

Almost thirty years ago, Richard Bird and Lambert Meertens developed a
framework for calculating functional programs from specifications, by
means of equational reasoning.  The specifications were usually
themselves functional programs, which were obviously correct, but
ridiculously inefficient.  They were then transformed, step by step,
by the application of a number of identities, into efficient and
elegant code, the stuff of many a "functional pearl" (the name of a
regular column published in JFP, the flagship journal of the
functional programming community).

There were two problems.  The first, that the identities had been
developed for the datatype of lists ([Bird 1986][TL]) and although it
seemed clear that they could be translated to other types, for
instance trees ([Bird 1988][LC]), it was not at all clear whether
there was a theory underlying the translation that could guide it (and
perhaps explain when it would work and when not).  The second problem
was that there were ''many'' identities, and it was not obvious how to
organize them so they could be remembered and used in a reasonable
way.

The solution to both problems turned out to be the same: category
theory provided both the framework for organizing the numerous
identities on lists ''and'' the instruments for their principled
translation to other datatypes ([Spivey 1989][CT], [Malcolm 1990][GM],
[Meijer et. al. 1991][BW]).  This was the start of many developments
which led to the introduction of elements such as the typeclasses
Functor or Monad in Haskell, and for which there is no end in sight.

The aim of this course is to give an overview of these developments,
from the beginning to the latest (not last!) word on the subject,
spoken by Hinze, Wu and Gibbons ([Hinze 2014][H14]).  Thus, this will
be a course with a clear focus on those parts of category theory which
are most relevant to program calculation, and with a large number of
applications.  Category theory is dauntingly general, and its other
applications to computer science are numerous and fascinating.  We
will resolutely resist this fascination, except for the occasional
historical remark and literature reference.

We shall begin with one or two lectures on program calculation in the
functional setting.  This will serve as a reminder to those students
who have seen this before, but can also function as an accelerated
introduction to the basic functional programming we need later (for
example, for Maths students who haven't taken functional programming
courses).

The rest of the lectures will cover the standard topics (categories,
functors, natural transformations, initial and final algebras, adjoint
functors, monads).  We'll use the first three chapters of
[Bird 1997][AOP], [Meertens 1995][LM], and, in the first part, Graham
Hutton's MGS lectures ([Hutton 2004][HT]) and the original papers,
which will be made available.

The ideal prerequisite is familiarity with functional programming and
an appreciation of calculational reasoning.  The latter is probably
more important than the former.

## Overview

The aim of this course is to introduce category theory as a framework
for calculating functional programs, from the very beginning to the
latest developments on the subject.

### Learning objectives

The goal of this course it to understand the latest developments in
the use of category theory in program calculation, as expressed in
[Hinze 2013][H13] and the not yet published [Hinze 2014][H14].

To achive this, students will have to be familiar with:

* categorical description of recursive datatypes, including nested datatypes and indexed datatypes
* categorical formulation of recursive schemes, including (but not limited to) catamorphism, anamorphisms, hylomorphisms, paramorphisms, and apomorphisms.
* the relationship, similarities and differences between Haskell constructs and the corresponding categorical ones (e.g., between the typeclass `Monad`  and the categorical monad).

### Examination

The course is examined through

* a sequence of hand-ins (solutions to exercises to be further specified during the course).
* active participation in most of the weekly seminars

### Contents

1. Calculating functional programs.
2. Categories.  Definition, examples.
3. Functors.
4. Natural transformations.
5. Initial algebras and final co-algebras.
6. Applications.
7. Adjoint functors and monads.
8. Adjoint folds.
9. Conjugate hylomorphisms.

### References

[TL]: Bird 1986, [Introduction to the Theory of Lists](https://www.cs.ox.ac.uk/files/3378/PRG56.pdf)

[LC]: Bird 1988, [Lectures on Constructive Functional Programming](https://www.cs.ox.ac.uk/files/3390/PRG69.pdf)

[CT]: Spivey 1989, [A Categorical Theory of Lists](http://link.springer.com/chapter/10.1007%2F3-540-51305-1_24)

[GM]: Malcolm 1990, [Algebraic Data Types and Program Transformation](http://cgi.csc.liv.ac.uk/~grant/Bib/thesis.html)

[BW]: Meijer, Fokkinga, Patterson 1991, [Functional programming with bananas, lenses, envelopes and barbed wire](http://link.springer.com/chapter/10.1007%2F3540543961_7)

[LM]: Meertens 1995, [Category Theory for Program Construction by Calculation](http://www.kestrel.edu/home/people/meertens/diverse/ct4pc.pdf)

[AOP]: Bird and de Moor 1997, ''The Algebra of Programming'', Princeton. (not online)

[HT]: Hutton 2002, [Introduction to Category Theory](http://www.cs.nott.ac.uk/~gmh/cat.html)

[H13]: Hinze 2013, [Adjoint folds and unfolds - An Extended Study](http://dx.doi.org/10.1016/j.scico.2012.07.011)

[H14]: Hinze, Wu, Gibbons 2014, [Conjugate Hylomorphisms‚ or: The Mother of All Structured Recursion Schemes](http://www.cs.ox.ac.uk/people/jeremy.gibbons/publications/conjugate-hylos.pdf)
