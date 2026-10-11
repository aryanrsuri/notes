# Modules and abstraction

## Decomposition and interface cost

### Can Great Programmers Be Taught?

https://youtu.be/LtRWu9DErgU?si=7yebqitDhwwxJMFy

- Elite programmers are >10x more productive
- How do you take a big problem, and partition it into solvable issues/requirements?
- Read `Talent is Overrated` * Colvin

> Knuth: Layers of abstraction

> John Ousterhout: Problem Decomposition

#### What are the *Secrets*?

- Classes should be deep
- General-purpose classes are deeper
- Working code isn't enough, you must minimise complexity
   - Complexity is derived from dependicies and obsfucation

Read `On the Criteria to be User in Decomposing Systems into Modules` by Parnas

```text
Deep 	|-------| <* Interface: User knowledge (cost)
Class   |	| }
        |	|  } * Functionality of the Class (benifit)
        |	| }

Shallow |-----------------------|
Class   |			|

Ideal 	|--|
Class   |  |
        |  |
        |  |
        |  |
```

- Length (LOC) isn't the important issue: it's *abstraction*.
- "Classes should be small" is the wrong approach, so chopping up and making more classes (`classitis`), creates more complexity.

## Generality

### Can Great Programmers Be Taught?

https://youtu.be/LtRWu9DErgU?si=7yebqitDhwwxJMFy

Approach...
(A) Start specialised, generalise later

- Issue, they start becoming quite complex, with info-leak
   --> (B) General-purpose design from the start
- Fewer methods
- Better modular decomposition

> Be `somewhat` general-purpose
- Focus on known needs
- Avoid specialisation

## Primitives and composition

E.g don't write one function for each key, make a `key_input` function

Implement the simplest possible module

Effectivily these become helper librarys, try and much many of these so
that you can *compose* them.

### Core

- What is the thing we are doing, how can we generalise what it does?
- Think about the **primitives** * the atomic construct. (i.e node for a DAG based visualy editor, or clips with parameters)
- There are also **structures** * the layer to operate on (i.e UNIX: cli to pipe , the primitive is files
- What are the garuntess? the **requirements** and the interface?

## Changing dependencies

We are optimising for:

- Dependability
- Extensibilty
- Team scaleability
- Development velocity

How do we *reduce* risk? What is the risk profile?

What *can* change?

- Platform
- Language implementations
- Hardware
- Priorities
- Team churn

Modules are black boxes, they are rock-solid and you only communicate
through a wide interface. Best way to design (e.g. large C codebase,
simple header file for others to use). `Writing` the application,
means composing these modules (abstractions). One writer for one module

Some modules are difficulty, soem are senior, some are junior. A module
can be exchanged without changing its interfaces. i.e rewrite a module,
then transition to it *over time*

### Architecting/Design

Develop a wrapper **around** things you can't control, i.e. providing
a wrapper around a platform layer (like termios, window open)

- Learn to think forward
- Avoid implementing *good-enough-for-now* (i.e technical debt [[design-investment-and-debt]])
   - *if you do* hid it behind a solid interface (black box)

## Reuse

### Advice for Writing Small Programs (in C)

1. Spend your time writing code that gets stuff done
1. Code reuse is **crucial**

### Cathedral and the Bazaar

1. Good programmers know what to write. Great ones know what to rewrite (and reuse).

1. Any tool should be useful in the expected way, but a truly great tool lends itself to uses you never expected.
