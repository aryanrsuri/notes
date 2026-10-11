# Making software simpler to understand and change

## Complexity and ease

Much of the discussions on complexity are similer to Hinley's talks

Abgridged:

- complexity is **not** difficulty
- complexity is **not** breadth
- complexity **is** the amount of internal interaction-the braiding.

- Out of the Tar Pit * Accidental v Essential complexity
- "Software architecture degrades [with] changes to the software..."

Simple made easy

- Simplicity is a choice
- Simplicity != Ease

- Simplicity is not a lack of cardinality, in fact more simplicity usually requires making more things

### Simple(x) (vs Complex)

Roots: are *sim* & *plex*
Meaning: One fold or braid

The opposite of simple/simplex is *complex* e.g many folds or braids

Orthogonal to Simplex is Easy

#### Easy (vs Hard)

Roots: are the french _aise_ or adjacent
Meaning: to lie nead

The antonym to easy is hard (meaning strong very strong)

#### Simple

One fold/braid (focus of) e.g.:

- one role
- one task
- one concept
- one dimension
Not:

- one instance
- one operation

Simple focus the lack of interleaving, not lack of *cardinality*

Critical: Simple is an **objective** concept, we can investegatek the braiding

#### Complex

Many braids. fully opposite to simplex

The source of complexity is the act of **complect**, which means to interleave or braid something.

#### Easy

Near, at hand, e.g.:

- near our ide, repo, package manager, disk, etc...
- near our understanding or skill set
   - Familiar * we are fixated on this concept and often *obfuscate* it with simplicity
- near our capabilities
   - there is always a limit, you can learn more things but to a saturation

Critical: Easy is a **relative** concept, since familiarity to oneself is relative

Nota bene that easy does not imply simplex, as so many constructs are familiary and availabe yet complex. What is important is the complexity they yield in the artifact, which is *incedental* (i.e. *your fault*)

- Ease of understanding
- Ease of change
- Ease of debugging
- Flexibility
   - Policy, Location, etc

## Understanding, change, and reliability

Critical: we can only make reliable those things we can understand

Nota bene, we can only consider a few things at a time (small number), and when things
are interleaved we need to pull in the two things, which further reduces our bandwith.
Complexity (interleaving) limits reasoning ability

(Think here of a juggler, maybe 3 things for 95%, the tail 99% best juggler maybe gets to 10 things, but >20 is impossible)

### Change

What will be impact, Where does that change need to hanppen
Critical: You must be able to **reason** about your construct

Every bug has passed the type checker and the tests. You can make an analogy of tests/type checker to guardrails when driving. You never rely on this, bump on them, to get anywhere. You must be able to reason (drive) your construct to conclusion.

- Testing, refactoring, type checking doesn't care, so do not rely on them

#### How to make things Easy

Bring closer:

- installing
- getting approved
- become familiary by learing
Mental capacity? (refer to the juggler analogy) this isn't going to move very far

## Constructs and artifacts

- Choose simple constructs over complexity-generating constructs
   - Its the artifacts, not the authoring
- Create abstractions with simplicity as bias

The sofware, language, etc is the construct:
But the actual product, the interfance the compiled code is the product
We should assess the construct by the artifact

### Construct

We focus too much on the experience of the construct:

- Programmer convenience
- Programmer replaceability/churn

#### Artifact

Long term results of use, attributes of the artifacts

- Software quality, correctness
- Maintenance, churn/change

## Development speed

Emphasising ease gives early speed, but over time, will substatniallty loever development speed. This is opposite to emphasising simplex. Effectiveiyl, with empahsising ease you get a _knitted castle_ something that interleaves

## Separating concerns

The myth is making composable, modular systems are simple. But paritioning and stratification don't imply simplicty

- They enable it but if dependence occurs simplex is hard

### Abstraction

Can help or hinder simplicity

Abstract means `to draw away`, thinkg about the who, what, where, when, why and how

#### What

- operations
- form abstractions from related SMALL sets of functions
   - these are specifications: inputs, outputs (only values and other abstractions)
- represent w/ polymorphism

#### Who

- entities implementing your abstractions
- built from subcomponents
#### How

- implementing logic
- connect to abstractions and entities via polymorphic constructs
- Again, don't write abstractions that already implement `how`
- don't complect with anything

#### When, Where

E.g a calls b and a requires c

- Really avoid complecting these with anything in the design
- Mainly enter via connected objects
   - Use queues:

#### Why

E.g the policy and rules strewn everyhitng

## Values, state, and implementation choices

Complex Alternatives

| Complexity | Simplicity |
| --- | --- |
| State Obj  | Values     |
| Methods    | Functions  |
| vars       | managed refs|
| inheritance, switch, matching | polymorphism a la carte |
| syntax | data |
| imperative loops | set functions |
| actors | queues |
| orm | data manipulation |
| conditionals | rules — * won't replace |
| inconsistency | consistency — * read up on eventual consistency |

### Even simpler constructs

| Construct             | Get it via            |
| --- | --- |
| values    | final persistanct collections     |
| functions | functions                         |
| namespaces | langauge support                 |
| data | structs (map, arr, set, json, etc)     |
| polymorphism | type classes                   |
| managed refs | haskell refs                   |
| set functins | lib                            |
| queues | lib                                  |
| data manipulation | sql                       |
| rules | lib                                   |
| consistency | transaction, values             |

#### State is never simple

It is *easy* (near you available) but it *complects* value and time

## Data and composition

### Simple Made Easy

Information/data is by nature simplex, do not complect it by hiding it behind a class w/ informational method, it poisins data composition

### Cathedral and the Bazaar

1. Smart data structures and dumb code works a lot better than the other way around.

1. When writing gateway software of any kind, take pains to disturb the data stream as little as possible—and never throw away information unless the recipient forces you to!

## Capacity and complexity

### Risk Homeostatis

Proposes that individuals have a preferred or "target level" of risk they are comfortable with and will adjust their behavior to maintain that level

People can handle more complexity as well, and can grow systems which invite *more* complexity, in a cycle.

## The Mess We're in

1. Code even you cannot understand a week after you wrote it--no comments or problem misunderstanding or ai-slop

1. Code that is shipped as soon as it runs and before it is beautiful
1. Code with added features
1. Code that is very very fast very very very obscure and incorrect
1. Code that is not beautiful
