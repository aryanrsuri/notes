# Specifications and program models

For any problem write a specification:

- a problem statement
- an enumeration of requirements
- an enumeration of assumptions for each requirement

This specification *could* be a spell ([[build-a-spellbook-of-methods-that-work]]) to put
in the spellbook.

tags: problems, solving, decomposition, computer-science, maths

Some questions:

- *what is the unkown?*
- what is required
- what do you want to find?

## Thinking Above The Code

Link: https://www.youtube.com/watch?v=-4Yp3j_jk8Q
Presenter: Leslie Lamport

> Writing is nature's way of letting you know how sloppy your thinking is
> * Guindon

To *really* think, you have to write

### What to write?

A blueprint: (In software) *Specifications*

### Specifications

There are **very** detailed blueprints-for a bridge lets say,
then on the other end is a rough sketch.

```text
Rough Sketch                Layout                   Very Detailed
|------------------------------|----------------------------|
Prose                Mathematical Prose              Formal Specification
```

This is based-usually-on the *complexity* of the system:

- Some prose is very simple.
- Most code is somewhat simple
- Some code is quite complex and simple (concurrent/distributed systems)

### How to write a Spec? Tools

- Think like a scientist
   - Making *mathematical models* of reality
- Astronomy
   - Reality: Moons, Stars, Tides, etc...
   - Model: Object with mass and position
- Computer Science
   - Reality: Digital Systems
- Model: Functions, Sequences of State

## Input-output models and their limits

Functions map an input to an output

Math is a set of ordered pairs:
`sq:R->R = {(0,0),(1,1),(2,4)....}`

Math def. goes far, but has limitations in CS:

- Functions in CS specifies *what* a program does, but not how
   - quicksort & bubblesort compute sorting function, but diferently
- Some programs don't map a domain->range
   - e.g. run forever or OS

## Execution as sequences of states

- A program execution is represented by a behavior
- A behavior is a sequence of states
- A state is an assignemnt of values to variables
- A program is modeled by a set of behaviors, representing possible executions

> GCD(12,18) is only one behavior
> (12,18)-->(12,6)-->(6,6)

A set of behaviors:

- Any set `B` of behaviors := all behaviors satisfying a safety propery *S* UNION all behaviors satisfying a liveness property `L`
   - Safety Property: False iff violated at some point in behavior
   - Liveness Property: See complete behavior to know if its false
- Safety property *S* is more important b.c. that is where errors occur

### Specify a Safety Property

- The set of possible states
- A next-state relation, all possible successor states

A model can be **deterministic**, if for any state, there are unique inputs that make Next true. Where as multiple next states for a current state (i.e multiple inputs lead to making Next true)

### Technical Specification

- You need a formal language
- Even if you can't specify *correctness* (e.g. What the user **wants**), a spec is (even more) important than if you could.

## The Mess We're in

1. Code with no specifications

1. Code that you wrote without understanding the problem
