# Sociable and solitary unit tests
https://martinfowler.com/bliki/UnitTest.html

"Unit Tests" definition varies and leads to confusion.

## Elements of Unit Tests

Common elements
* low level tests, focusing on a small part of the system.
* written by programmers
* faster than other tests

The big difference : Unit.
* in OOP, unit ~ class
* in Functional/procedural Programming, unit ~function

**In practice, the unit depends and is decided by the dev team**

> But really it's a situational thing - the team decides what makes sense to be a unit for the purposes of their understanding of the system and its testing. Although I start with the notion of the unit being a class, I often take a bunch of closely related classes and treat them as a single unit. Rarely I might take a subset of methods in a class as a unit. However you define it doesn't really matter.

## Solitary vs Sociable tests

![](https://martinfowler.com/bliki/images/unitTest/isolate.png)

**Solitary** : Fault tolerant, test doubles for dependencies.  
This sounds great but in practice it's often unnecessary (unless the dependency is non-deterministic/slow - http calls, remote systems-).

> We didn't find it difficult to track down the actual fault, even if it caused neighboring tests to fail. So we felt allowing our tests to be sociable didn't lead to problems in practice.

**Sociable** unit tests do not fake the dependencies. Unit is not a code unit a behaviour unit.

Mock it or not depends is not a religion but should be a choice taking into account the stability and the speed of the dependency.

## Speed

* *Compile suite* run several times per minute on a programmer local workstation. Real time when developing.
* *Commit suite* run on the CI/CD and takes longer.

Duration threshold is subjective but the suite notion is shared.
