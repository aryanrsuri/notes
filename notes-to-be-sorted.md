=====
Notes
=====

Fragements * Me
-----------------
Testing [[programming-as-theory]] 
How **serious** am I? What to me is **sacred**? How far am I 
willing to go for what I want, and how little am I willing 
to compromise?

Being precise, terms to help me:
        * Serious
        * Problem (what *is* one, how to identify them)
        * Statement
        * Requirement
        * Assumption
        * Solution 
        * Hypothesis
        * Ontology
        * Theory
        * Spell / Procedure 
                * (pl) Spellbook / Manual
        * First Principle(s)
        * Abstraction
        * Component / Primitive
        * Construct
        * Artifact
        * Simple (Simplex) / Complex 
        * Fold / Interaction / Loop / Interleaving / Braid

Design is effectively choosing the best possible
components from the universe of first principle
derived components.

For any problem write a specification:
* a problem statement
* an enumeration of requirements
* an enumeration of assumptions for each requirement

This specification *could* be a spell to put 
in the spellbook.


Talent
----------

What is talent?

  I know that talent doesn’t feel like you’re amazing.
  It feels like the difficulties that trouble others are mysteriously absent in your case. Don’t ask yourself where your true gifts lie. Ask what other people seem weirdly bad at.


Observability 
------------

tags: tech

* Instrument (track, measure & log) everything
* Treat the logs, data, and monitoring as a product --> Inference team

Can I be a founder? * Sam Altman
----------------------------------
1. Four key traits
   1.1 Obsession
   1.2 Focus
   1.3 Frugality
   1.4 Love
2. Intelligence
3. Evangelism
4. Execution / Iteration speed
5. High rate of improvement
6. A true *mission*, motivation, a reason for founding.

Conflict
-----------

Conflict avoidance slowly erodes your life - squash your beefs.

  1. Conflict Recognition: your personal barometer of which situations, or 
     circumstances are conflict or stress.
  2. Conflict Holding: your ability to withstand or site in the presence of 
     conflict once you have recognised it.

How to solve it
------------------

tags: problems, solving, decomposition, computer-science, maths

Some questions:
* *what is the unkown?*
* what is required
* what do you want to find?
* 

On Problems
---------------

  *Have you tried solving the problem?*

Don't stroke the problem, thinking *about* the problem 
doesn't get you any closer to solving it.

How well do you notice problems and how serious do you take them?

Hard Work and Difficult Problems
***********************************

Hard Work and Difficult Problems are generally not closely related, and are separate.
Since difficulty problems require a lot of cognitive load, you cannot do it in a negative
mind place, but you can often do hard work while distracted-for example.

Hard Work
        Must put a lot of time and effort into it

Difficult Problem
        Must put a lof of skill or thinking into it

What can make a problem difficult:

a) Involves many desicions
b) !! The outcome depends *crucially* on the decisions made

Also prioritising desicsions that optimise for the solution needed

        Effective strategies often consist of converting difficult 
        problems into something that can be solved with hard work.

Elon on Solving Problems
****************************

* First principles analysis
* The only law is the law of phsyics, everything else is a recommendation

When solving a problem look at its consisteuent primitives, and go from there.
Example is looking at the weights of the raw materials and prices and that is 
the **magic wand** price (if you can wave a wand and arrage the atoms into a product)

Don't use your precoinved biases to determine the product, go from the 
*platonic* idea of the theoritcal perfect product, and try to get the
atoms in that shape.

Weak/Strong-Linked Problems
*****************************

Weak-link problems are those where the overall quality depends on how good the *worst* stuff is
Strong-link problems are those where the overall quality depends on how good the *best* stuff is

Science is a strong-link problem, don't focus on short-term, or timid, or done-before; try to get
*wierd*, *new*, and serious about something in Science that can become an outlier. Accept risk, 

Solving and Dissolving Problems
************************************

There is **solving** and **dissolving** the problem.

Dissolving
  If a problem is made to go away without solving it. Arranging things in such a way
  that you don't have the problem

NOT the same as "avoiding" problems.

Being Serious
---------------

TL;DR
******

Be serious about **something**-You must hold *something* sacred.

-----

Seriousness tells you what to keep and give up

Three lies they tell you to *stop* being serious:

1. Seriousness is all or nothing.
        1.1 Simple question to those: “What’s the tiniest change you’re willing to make right now, today, and that you can make slightly larger tomorrow?”
2. You have to be serious about everything at once
3. You are only serious about something if you are getting paid to do it.

        There’s a devastating scene in Succession where the 
        billionaire Logan Roy tells his adult children, all
        of whom are failures in different ways: “You are not serious people.”

        “Serious”—what a perfect word. Not in the sense of 
        grim or unfunny. More in the sense that means it: 
        something like, “actually caring about stuff, and 
        for the right reasons.”

        Before that, I believed what everybody else seems
        to believe: if you play the game well enough and
        long enough, eventually you get to stop playing 
        and go do whatever you want. I played the game 
        pretty well for a long time, and now it’s obvious
        to me that the reward for playing the game is more game.
        You just keep unlocking levels forever, and the levels 
        don’t even get more interesting (“Ooh, this one is in space!”).
        It’s just the same thing over and over until you die.
        You don’t get out by winning; you get out by stopping.

        So seriousness isn’t some kind of final reward, a golden
        watch you earn for a lifetime of operating in bad faith.
        It is, instead, one of those basic practices you gotta do 
        to prevent your life from disintegrating, like getting out
        of bed and taking a shower and talking to people. That’s
        because seriousness is the great Orderer of Priorities, and the Priorities must be Ordered. Otherwise, they grow flabby and unkempt, and you’ll find yourself doing something stupid like working some job you mildly detest or scrolling on your phone, and the next time you look up, seventy years have passed, and now you’re just a skeleton, dead before you ever got around to living.



Embrace the grind * Jacob Kaplan Moss
----------------------------------------

        Being willing to do something so terrifically tedious that it appears to be magic — works in tech too.

        I merely did something so boring that nobody else had been willing to do it.


Architecting Large Software Projects
------------------------------------------

        Write code so it never breaks

        Its faster to write ``N`` lines of code today,
        Than write ``k << N`` lines of code today, and edit later.

We are optimising for:

* Dependability
* Extensibilty
* Team scaleability
* Development velocity

How do we *reduce* risk? What is the risk profile?

What *can* change?

* Platform
* Language implementations
* Hardware
* Priorities
* Team churn

!!! One of the most common sources of bugs in a badly architected (lots of moving parts system) is user error.
since bad architecuture makes constraint fails visible and doable by the user.

Modules 
**********
Modules are black boxes, they are rock-solid and you only communicate 
through a wide interface. Best way to design (e.g. large C codebase,
simple header file for others to use). ``Writing`` the application,
means composing these modules (abstractions). One writer for one module 

Some modules are difficulty, soem are senior, some are junior. A module
can be exchanged without changing its interfaces. i.e rewrite a module,
then transition to it *over time*

Architecting/Design
********************

Develop a wrapper **around** things you can't control, i.e. providing
a wrapper around a platform layer (like termios, window open)

* Learn to think forward
* Avoid implementing *good-enough-for-now* (i.e technical debt)
        * *if you do* hid it behind a solid interface (black box)

Try to write a test application:

* Minimal
* Logging
* Portable



Consolidate functionality
^^^^^^^^^^^^^^^^^^^^^^^^^^

E.g don't write one function for each key, make a ``key_input`` function

Implement the simplest possible module

Effectivily these become helper librarys, try and much many of these so
that you can *compose* them.

Core
^^^^^^

* What is the thing we are doing, how can we generalise what it does?
* Think about the **primitives** * the atomic construct. (i.e node for a DAG based visualy editor, or clips with parameters)
* There are also **structures** * the layer to operate on (i.e UNIX: cli to pipe , the primitive is files
* What are the garuntess? the **requirements** and the interface?


David R. MacIver
------------------

Action Generators
******************

Action Generator
        Something that prompts you to act in the world

They can have one of two results:
        a) Do *nothing*
        b) Do *something*:
                i) Set of actions it *can* generate
                ii) Subset of actions it *encourages* you to take

Theories act as action generators

        It’s worth having a stable of bad theories lying around that
        generate actions that you wouldn’t otherwise have thought of
        and that are basically harmless in the worst case, and possibly
        interesting in the best case.

The Manual that solves all your problems
*******************************************

        “That seems like a problem. Have you tried solving it?” 
        is one of my catch phrases, and I think one helpful way to 
        start on something like this is “If I looked in the Manual,
        what would it tell me to do?”

        Another very general purpose procedure is “Write down all 
        the steps you need to perform to do the thing in enough 
        detail that you have no uncertainty left.”9

        but real expert decision making isn’t this sort of formalised 
        decision tree of if A then do B else do C, it’s **pattern matching based**.
        You see a situation, it reminds you of something, you 
        consider doing the thing that your experience 
        suggests is a good idea from that. Then you critique the 
        suggestion and discard it if it doesn’t work. This is what 
        expertise looks like.

        This means that when you encounter a novel problem you can try
        to go “OK, what procedure do I apply to this?”

        This may or may not work, but you win either way: Either you 
        achieve something, or you learn something more about the procedure
        and where it’s useful. This might result in you refining it further,
        or it might result in you realising something about its limitations
        or the nature of the problem that mean it can’t work, which will let 
        you avoid using it where you shouldn’t in future. It might also just 
        mean you need to practice it more.

Do a final retrospective after applying the procedure (which *ultimately* may
-or may not-have worked) to analyse "Why did this work / not work? What can I
learn from that? Was that what the manual asked me to do?" If no then iterate
on it.

        If it is yes-you have glimpsed an aspect of the **divine**.

Magical practice about the Manual
************************************

Spell
        A procedure that works: codified and given a name

* Procedures == *Spells*
        * When a procedure works, codify it, give it a name, and call it a spell
        * Iterate on the spell design to improve it

Example(s) of a Spell (for writing the newsletter)

#. Put a timer on, and work on a well-defined task
        a) prefer physical objects
        b) avoid **choice points** where you don't need them
        c) don't introduce unpleasant elements
#. Put on noise-canceling headphones for working
        a) What sort of headphones?
        b) What do you listen to?

These can be very thorough

Attention Management Spell
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Get something that is weighty and fidget-able (a cube?), this 
is your **secondary anchor**.

Then the **primary anchor** is the thing you ar eintending to focusing on
-your task.

Your allocated task-span (the pomodoro spell) is to either:
        a) Work on your primary anchor (task)
        b) Notice you aren't and fidget with secondary anchor (its own spell)
                * This is **NOT** negative
                        * If frustrated with this, don't immediately
                          switch back. Calm, breathe, and do somethign
                          with your secondary anchor
                * If you spend your whole time-span on this,
                  you have learnt something important
                * You can pick up the sec. anchor any time, but only
                  put it down **in order to resume the prim. anchor**

We un-conciously *do* have a set of tools/procedures we apply, but 
codifying them, and thinking about them help improve them-its a positive
cycle.

Turning skill learning: am I doing ``X`` well? becomes:
        1. Which of the spells ``S`` should I apply to X
        2. How do I do ``S`` well?

You effectively turn ``X`` into a continous problem space (Vector space/Universe) of all
morphisims , ``f``, that map a spell ``S`` to a solution to some aspect 
of X ``X``, or ``F{f}: S -> X``. These spells are then distinct objects you can
practice.

        If you want to get better at life then, when you encounter a problem, solve it.

Anchors 
^^^^^^^^
Refactor from shiny things --> anchors. Anchors and be good or bad, simply something 
our attention *usually* drifts towards, another term might be sinks/black holes.

Anchors usually follow **down** the energy gradient, that is, it takes less effort to
move attention to this thing than what you are currently doing.

        The question is how to turn desired focus of work into an anchor?

Most spells are 
        
        I am in state X, how to get to state Y?

We can instead of going from non-focused to focused on, use transistion states

        ``Y > X_1 > X``

And so anchors, secondary, can be **that transistionary state**

.. image::
   https://substack-post-media.s3.amazonaws.com/public/images/abe2cf6c-202f-4591-a089-a72f9dd7220d_193x251.png
   width: 400

#. Start a spellbook 
#. Whenever you have a problem (Being concious about your life here helps)
try to figure out a spell for solving it. This includes spells you already
have
#. Learn from this and do better
#. (Talk to others about their spells)


Can Great Programmers Be Taught?
---------------------------------
https://youtu.be/LtRWu9DErgU?si=7yebqitDhwwxJMFy


The most important concept in CS?
*********************************
* Elite programmers are >10x more productive
* How do you take a big problem, and partition it into solvable issues/requirements?
* Read `Talent is Overrated` * Colvin

    Knuth: Layers of abstraction

    John Ousterhout: Problem Decomposition

What are the *Secrets*?
****************************

* Classes should be deep
* General-purpose classes are deeper
* Working code isn't enough, you must minimise complexity
        * Complexity is derived from dependicies and obsfucation
* There exists ``Strategies`` versus ``Tactical`` programming

Classes should be deep
****************************

Read ``On the Criteria to be User in Decomposing Systems into Modules`` by Parnas

.. code:: text

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

* Length (LOC) isn't the important issue: it's *abstraction*.
* "Classes should be small" is the wrong approach, so chopping up and making more classes (`classitis`), creates more complexity.

General-purpose classes are deep
**************

Approach...
(A) Start specialised, generalise later
* Issue, they start becoming quite complex, with info-leak
--> (B) General-purpose design from the start
* Fewer methods
* Better modular decomposition

	Be `somewhat` general-purpose
* Focus on known needs
* Avoid specialisation

(Mindset) Tactical vs Strategic Programming
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tactical
^^^^^^^^
* Get next feature/bug-fix working
* A few shortcuts and kludges are **OK**
* Result --> Bad design with high complexity
* Complexity is Incremental, death by one-thousand cuts
* Extreme: Tactical Tornadoes (Literally Me)
        * Can ship extremely fast, get the next feature or bug-fix done, land the PR
        * The problem is they get things 80% done, use shortcuts, slop, or kludges, and leave a mess of debt
* Most startups are tactical, and `clean later`, but code becomes spaghetti. Facebook is a great example
        * Move quickly and break things
        * eventually realised
        * Move quickly with solid infrastructure

Strategic
^^^^^^^^^^
* Produce a great design
* Simplify future development
* Minimise complexity, "sweat the small stuff"
* Investment mindset: Take more time now, pay back later

How much to Invest?
^^^^^^^^^^^^^^^^^^^^^^
* Make continual small improvements, ~20% overhead
* When writing new code:
        * Careful design
        * Good documentation
* When changing new code:
        * After change, system is the way it *would* have been designed if that way from the start
        * Always find something to improve
* Ask yourself: Is this the most I can afford to invest right now?

Thinking Above The Code
-----------------------
Link: https://www.youtube.com/watch?v=-4Yp3j_jk8Q
Presenter: Leslie Lamport

        Writing is nature's way of letting you know how sloppy your thinking is
        * Guindon

To *really* think, you have to write

What to write?
*************************
A blueprint: (In software) *Specifications*

Specifications
*************************
There are **very** detailed blueprints-for a bridge lets say,
then on the other end is a rough sketch.


.. code:: text

        Rough Sketch                Layout                   Very Detailed
        |------------------------------|----------------------------|
        Prose                Mathematical Prose              Formal Specification

This is based-usually-on the *complexity* of the system:
* Some prose is very simple.
* Most code is somewhat simple
* Some code is quite complex and simple (concurrent/distributed systems)

How to write a Spec? Tools
~~~~~~~~~~~~~~~~~~~~~~~~~~~
* Think like a scientist
        * Making *mathematical models* of reality
* Astronomy
        * Reality: Moons, Stars, Tides, etc...
        * Model: Object with mass and position
* Computer Science
        * Reality: Digital Systems
* Model: Functions, Sequences of State

The Function(al) Model
**********************
Functions map an input to an output

Math is a set of ordered pairs:
``sq:R->R = {(0,0),(1,1),(2,4)....}``

Math def. goes far, but has limitations in CS:
* Functions in CS specifies *what* a program does, but not how
        * quicksort & bubblesort compute sorting function, but diferently
* Some programs don't map a domain->range
        * e.g. run forever or OS

The Standard Behavioral Model
*************************************
* A program execution is represented by a behavior
* A behavior is a sequence of states
* A state is an assignemnt of values to variables
* A program is modeled by a set of behaviors, representing possible executions

        GCD(12,18) is only one behavior
        (12,18)-->(12,6)-->(6,6)

A set of behaviors:
* Any set ``B`` of behaviors := all behaviors satisfying a safety propery *S* UNION all behaviors satisfying a liveness property ``L``
        * Safety Property: False iff violated at some point in behavior
        * Liveness Property: See complete behavior to know if its false
* Safety property *S* is more important b.c. that is where errors occur

Specify a Safety Property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
a) The set of possible states
b) A next-state relation, all possible successor states

A model can be **deterministic**, if for any state, there are unique inputs that make Next true. Where as multiple next states for a current state (i.e multiple inputs lead to making Next true)

Technical Specification
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
* You need a formal language
* Even if you can't specify *correctness* (e.g. What the user **wants**), a spec is (even more) important than if you could.

How to not be a noob
-------------------------
https://youtu.be/-v8pD0d5Bmk?si=fAlKOI5k3IUEtnjZ

* Don't *think* like a noob
* Think *outside* the rectangular grid

How to stand out without trying hard
--------------------------------------
* Potential is performance trend *over* time
* People who take ownership, are marked as high performers
* Its about how quickly you can learn new things

Technical Debt
------------------
https://martinfowler.com/bliki/TechnicalDebt.html

https://youtu.be/ukgmp6uxQJc?si=B-NwkKLqhFw4ECvd

https://sites.google.com/site/unclebobconsultingllc/a-mess-is-not-a-technical-debt

        software systems are prone to the build up of **cruft**
        -deficiencies in internal quality that make it harder than
        it would ideally by to modify and extend the system further.
        Martin Fowler

Ultimately it is a tradeoff, but the best is if there are
high cruft, high stable areas of the codebase you can avoid
paying this debt. Conversly, high-churn parts of the codebase
we should **abjure** the presence of debt.

..  Uncle Bob argues that

                        A mess is not a debt
                        -* Uncle Bob

        i.e that bad code (produced by lack of good sofwtare design)
        isn't a *debt* but a loss-a mess. Technical debt (in Bob's POV)
        should be concious decisions based on project constraints, and
        risky. Messes are *not* rational, as debt should be.

        **Fowler's Response**

        Not exaclty, technial debt is a metaphor, and thus it is not about
        whether a flaw is debt *or not*, but wether the metaphor is helpful.
        Messy code *is* a debt, but reckless and bad.

It's often the case that it can take a year of programming on a project
before you understand what the best design approach should have been.

Thus, it becomes a x-y graph

.. code:: text
                        Deliberate
                           |
        -x(Reckless)-------|-------(Prudent)+x
                           |
                        Inadvertent

        -x+y (We don't have time for design)
        -x-y (What's layering?)
        +x+y (We must ship now and deal with the consequences)
        +x-y (Now we know how we should have done it)

.. image:: https://martinfowler.com/bliki/images/design-stamina-hypothesis/graph.png
   :width: 800


Why can't we make *simpler* software?
--------------------------------------

Much of the discussions on complexity are similer to Hinley's talks

Abgridged:

* complexity is **not** difficulty
* complexity is **not** breadth
* complexity **is** the amount of internal interaction-the braiding.

Model/Reality
**************

* The model doesn'y *actually* map onto the problem domain.
* When your problems multiply because of above you get a hyperspace of complication


Risk Homeostatis
****************

Proposes that individuals have a preferred or "target level" of risk they are comfortable with and will adjust their behavior to maintain that level

People can handle more complexity as well, and can grow systems which invite *more* complexity, in a cycle.

Theory of Complexity
*********************

* Out of the Tar Pit * Accidental v Essential complexity
* "Software architecture degrades [with] changes to the software..."

Advice for Writing Small Programs (in C)
------------------------------------------

TL;DL
******

1. Spend your time writing code that gets stuff done
2. Code reuse is **crucial**


.. rubric :: Footnotes


----


Simple Made Easy
--------------------
Simple made easy

* Simplicity is a choice
* Simplicity != Ease
* Testing, refactoring, type checking doesn't care, so do not rely on them
* Choose simple constructs over complexity-generating constructs
  * Its the artifacts, not the authoring
* Create abstractions with simplicity as bias
* Simplify the problem space before you start
* Simplicity is not a lack of cardinality, in fact more simplicity usually requires making more things


Word Precision
******************

Simple(x) (vs Complex)
~~~~~~~~~~~~~~~~~~~~~~~~

Roots: are *sim* & *plex*
Meaning: One fold or braid

The opposite of simple/simplex is *complex* e.g many folds or braids

Orthogonal to Simplex is Easy

Easy (vs Hard)
~~~~~~~~~~~~~~~~~~~~~~~~

Roots: are the french _aise_ or adjacent
Meaning: to lie nead

The antonym to easy is hard (meaning strong very strong)

Simple
~~~~~~~~~~~~~~~~~~~~~~~~

One fold/braid (focus of) e.g.:
  * one role
  * one task
  * one concept
  * one dimension
Not:
  * one instance
  * one operation

Simple focus the lack of interleaving, not lack of *cardinality*

Critical: Simple is an **objective** concept, we can investegatek the braiding

Complex
~~~~~~~~~~~~~~~~~~~~~~~~

Many braids. fully opposite to simplex

The source of complexity is the act of **complect**, which means to interleave or braid something.

Easy
~~~~~~~~~~~~~~~~~~~~~~~~

Near, at hand, e.g.:
  * near our ide, repo, package manager, disk, etc...
  * near our understanding or skill set
    * Familiar * we are fixated on this concept and often *obfuscate* it with simplicity
  * near our capabilities
    * there is always a limit, you can learn more things but to a saturation

Critical: Easy is a **relative** concept, since familiarity to oneself is relative

Nota bene that easy does not imply simplex, as so many constructs are familiary and availabe yet complex. What is important is the complexity they yield in the artifact, which is *incedental* (i.e. *your fault*)


Working with Simple and Easy: Using Contructs and Artifacts
************************************************************************

The sofware, language, etc is the construct:
But the actual product, the interfance the compiled code is the product
We should assess the construct by the artifact

Construct
~~~~~~~~~~~~~~~~~~~~~~~~

We focus too much on the experience of the construct:
  * Programmer convenience
  * Programmer replaceability/churn

Artifact
~~~~~~~~~~~~~~~~~~~~~~~~

Long term results of use, attributes of the artifacts
  * Software quality, correctness
  * Maintenance, churn/change

Limits
~~~~~~~~~~~~~~~~~~~~~~~~

Critical: we can only make reliable those things we can understand

Nota bene, we can only consider a few things at a time (small number), and when things
are interleaved we need to pull in the two things, which further reduces our bandwith.
Complexity (interleaving) limits reasoning ability

(Think here of a juggler, maybe 3 things for 95%, the tail 99% best juggler maybe gets to 10 things, but >20 is impossible)

Change 
~~~~~~~~~~~~~~~~~~~~~~~~

What will be impact, Where does that change need to hanppen
Critical: You must be able to **reason** about your construct

Debugging
~~~~~~~~~~~~~~~~~~~~~~~~

Every bug has passed the type checker and the tests. You can make an analogy of tests/type checker to guardrails when driving. You never rely on this, bump on them, to get anywhere. You must be able to reason (drive) your construct to conclusion.

Development Speed
~~~~~~~~~~~~~~~~~~~~~~~~

Emphasising ease gives early speed, but over time, will substatniallty loever development speed. This is opposite to emphasising simplex. Effectiveiyl, with empahsising ease you get a _knitted castle_ something that interleaves

Benifits of simplicity
~~~~~~~~~~~~~~~~~~~~~~~~

 * Ease of understanding
 * Ease of change
 * Ease of debugging 
 * Flexibility
    * Policy, Location, etc


How to make things Easy
**************************

Bring closer:
  * installing
  * getting approved 
  * become familiary by learing
Mental capacity? (refer to the juggler analogy) this isn't going to move very far

Examine your toolkit
~~~~~~~~~~~~~~~~~~~~~~

Complex Alternatives

| Complexity | Simplicity |
|-------------------------|
| State Obj  | Values     |
| Methods    | Functions  |
| vars       | managed refs| 
| inheritance, switch, matching | polymorphism a la carte |
| syntax | data |
| imperative loops | set functions
| actors | queues |
| orm | data manipulation |
| conditionals | rules | * won't replace
| inconsistency | consistency | * read up on eventual consistency

Even simpler constructs
~~~~~~~~~~~~~~~~~~~~~~

| Construct             | Get it via            |
|-----------------------------------------------|
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

Modularity and Simplicity
*****************************

The myth is making composable, modular systems are simple. But paritioning and stratification don't imply simplicty
  * They enable it but if dependence occurs simplex is hard

State is never simple
*****************************

It is *easy* (near you available) but it *complects* value and time

Abstraction
*****************************

Can help or hinder simplicity

Abstract means `to draw away`, thinkg about the who, what, where, when, why and how

What
~~~~~
 * operations
 * form abstractions from related SMALL sets of functions
    * these are specifications: inputs, outputs (only values and other abstractions)
 * represent w/ polymorphism

Who
~~~~~

 * entities implementing your abstractions
 * built from subcomponents
How
~~~~~
 * implementing logic
 * connect to abstractions and entities via polymorphic constructs
 * Again, don't write abstractions that already implement `how` 
 * don't complect with anything

When, Where
~~~~~~~~~~~~~~~

E.g a calls b and a requires c
 * Really avoid complecting these with anything in the design
 * Mainly enter via connected objects
    * Use queues:

Why
~~~~~~~~~~~~~~~

E.g the policy and rules strewn everyhitng

Information *is* simple
~~~~~~~~~~~~~~~

Information/data is by nature simplex, do not complect it by hiding it behind a class w/ informational method, it poisins data composition

The Mess We're in
------------------

Seven deadly sins
********************
1. Code even you cannot understand a week after you wrote it--no comments or problem misunderstanding or ai-slop
2. Code with no specifications
3. Code that is shipped as soon as it runs and before it is beautiful
4. Code with added features
5. Code that is very very fast very very very obscure and incorrect
6. Code that is not beautiful
7. Code that you wrote without understanding the problem

How to be Cracked
----------------------
tags: peripherals, cracked, things, products

Physicality
*************

* Good Posture
* Herman Miller chair
* Split Keyboard
* Wired headset w/ mic

Stack
*************

Tech
~~~~~~~~~~
* Python w/ Poetry
* Bash (zsh is fine)
* C++ / Cmake / Googletest
        * Will use golang

Knowledge Domains
~~~~~~~~~~~~~~~~~~~~
* OS
* Networking
* Software Design and Patterns
* Computer Architectures
* Distribute Systems
* ***Debugging Skills***
* Optimisation 

Streams
~~~~~~~~~~~~~~~~~~~~
* gRPC
* Protobufs
* Apache:
  * Kafka
  * Airflow
  * Spark
  * Parquet/Arrow
  * Cassandra

Application
~~~~~~~~~~~~~~~~~~~~
* Monitoring
  * Grafana
  * Prometheus/InfluxDB
* Logging:
  * Kibana stack:
    * Log->Logstash->Elastic->Kibana
  * Human readable and Binlogs
* Sensu
* Git

Environment
~~~~~~~~~~~~~~~~~~~~
* Vim+Tmux
* Linux/MacOS
* Docker

DB Layer
~~~~~~~~~~~~~~~~~~~~
* Timeseries
  * DolphinDB
  * InfluxDB
  * TimescaleDB
* NoSQL
  * Cassandra
  * MongoDB
* SQL
  * MySQL
  * PostreSQL

How to Focus
--------------

Artifacts of bad focus
*************************

* Busy but not effective
* Doing at lot, not getting a lot done
* Todo Lists and Schedules ad nauseam
* The justification of (and `need` to) multitask * the need to respond to teams messages mid meeting and such no true mono-focus

Constructs of good focus
*************************

1. Treat your brain like a toddler with a nice * fix your enviornments to be distraction free
2. Set stupidly small goals * trick your brain and let if build momentum
3. PROTECT YOUR ENERGY * Not a notifaction centre
4. Stop romantisicing burnout
5. Monotask like your life depends on it

Tiny Wisdoms
*************************

* You need clarity
* "You fall to the level of your systems"
* You control your actions of your technology 

Truth Drop
*************************

* What would my life look like if I finished what I started?

Official Prescription
*************************

1. Throw your phone across your room
2. Drink water
3. Start one _single_ thing, ride momentum

`Not today` say to brain when it tries to veer off

Cathedral and the Bazaar
-------------------------
tags: software, technical
1. Every good work of software starts by scratching a developer's personal itch.
2. Good programmers know what to write. Great ones know what to rewrite (and reuse).
3. Plan to throw one [version] away; you will, anyhow 
   (copied from Frederick Brooks's _[The Mythical Man-Month](https://en.wikipedia.org/wiki/The_Mythical_Man-Month "The Mythical Man-Month")_).
4. If you have the right attitude, interesting problems will find you.
5. When you lose interest in a program, your last duty to it is to hand it off to a competent successor.
6. Treating your users as co-developers is your least-hassle route to rapid code improvement and effective debugging.
7. [Release early. Release often.](https://en.wikipedia.org/wiki/Release_early,_release_often "Release early, release often") 
   And listen to your customers.
8. Given a large enough beta-tester and co-developer base, almost every problem will be characterized quickly and the fix obvious to someone.
9. Smart data structures and dumb code works a lot better than the other way around.
10. If you treat your beta-testers as if they're your most valuable resource, they will respond by becoming your most valuable resource.
11. The next best thing to having good ideas is recognizing good ideas from your users. Sometimes the latter is better.
12. !!! Often, the most striking and innovative solutions come from realizing that your concept of the problem was wrong.
13. !!! Perfection is achieved not when there is nothing more to add, but rather when there is nothing more to take away. 
    (Attributed to [Antoine de Saint-Exupéry](https://en.wikipedia.org/wiki/Antoine_de_Saint-Exup%C3%A9ry "Antoine de Saint-Exupéry"))
14. Any tool should be useful in the expected way, but a truly great tool lends itself to uses you never expected.
15. When writing gateway software of any kind, take pains to disturb the data stream as little as possible—and never throw away information unless the recipient forces you to!
16. When your [configuration] language is nowhere near [Turing-complete](https://en.wikipedia.org/wiki/Turing_completeness "Turing completeness"),
    [syntactic sugar](https://en.wikipedia.org/wiki/Syntactic_sugar "Syntactic sugar") can be your friend.
17. A security system is only as secure as its secret. Beware of pseudo-secrets.
18. To solve an interesting problem, start by finding a problem that is interesting to you.
19. Provided the development coordinator has a communications medium at least as good as the Internet, and knows how to lead without coercion, many heads are inevitably better than one.


Promoted quicker and be effective earlier in a company
--------------------------------------------------------
tags: career, people, lop, promotion, promoted, 1 on 1, 1:1
, startup, questions

Questions to ask in 1:1
*************************

1. “What’s the one thing you wish more people would ask you?"
2. "In your mind, what are the two most important things this quarter, this month, and this week"

----------

How to work within a Startup
----------------------------------

1. Prioritise the **right** high-value thing, and be clear 
that that's what you are doing.
2. Find problems, but bring solutions


Being effective early when joining a company
*********************************************

1. Aquire as *little* information as possible
        1.1 Forces you to learn the *right* information
        1.2 Forces you to do thinkgs you can actually achieve soon
        1.3 Prevents you from being distracted my the immensity of the task
2. Acquire information as efficiently as possible
        1.1 (Spell) Look at spellbook for ``Knowledge Acquisition``
3. Use the information you acquire as effectively as possible
        3.1 Value of Knowledge is effectively:
                3.1.1 If I do X, what is the outcome (X -> R) ?
                        3.1.1.1 Solve by Mental Models (f:X->R)
                                i. Implicit f: Black box; You know the answer without
                                and explicit description of the function (intuition)
                                ii. Explicit f: Think through all steps to reach the outcome. Typically
                                more work and more accurate, and articulate-able
                3.1.2 If I want Y, what should I do?
                        3.1.2.1 Answering this, is looking at 
                        the universe of {f:X->R}->Y. Everything else
                        is a optimisation for that search function
                                i. Generate ideas (using f:X->Rs and first-principles) of X->Rs
                                 and sort by what could work
                                ii. Put proper though into your *candidates* and decide
                                which is the best



Notes from "7 levels of Enginers" YT Video
************************************************

* Setting the engineering culture
* At high levels, technical communication is paramount
* Teamwork, since "you can go fast, or you can go far"
* Have a deep understanding of the business (time-in-role), look for opportunities for impact
        * With earning enough scope

Terms 
********

* Signal: useful and actionable information that helps you make desicions
* Surface: Some product artifact
* Scope: boundaries and definition of the product inlcusion/exclusion-the What
* Blast radius: impact caused by a change/person
* Land: merge/deliver a charnge or product

Company Choices
****************

* Pick the product/stack where the impact is
* "How did u get 2 year project in 6 months"
  * Cut some scope
  * Chatted w/ group and got hungry and excited about the project
* When looking at a huge scope
  * Showing that huge scope can even defeat morale so look at the edges/building blocks to deliver first 
* "What systems allow you to have work-life balance"
  * No meeting til after lunch
  * Wed/Fri no meetings
  * 1/1 on monday afternoon 
* PR Reviews
  * On low risk reviews be more high levels and rubber-stamp it
  * On high risk/prod refactors more thorough reviews
  * Defer to how do I accept this diff "what is absolutely blocking this thing from going to prod"
* if you aren't getting negative feedback on pm then keep pushing the $[edge] / boundary of speed
* go where you are rare
* note taking system:
  * txt doc new readme file [current project name]
  * insert datetime to index on that
  * linkes between the file.
  * Root files:
    * priorities
    * memos/quotes
  * launch post for projects
* Go where you are **valued**

Progression & Manager-Employee Relationship
********************************
* Be honest with your manager about what you will do **trust** is both ways.
* $[Brag List] Keep a notebook of things that will be helpful in summarising for Performance Reviews.
  * Bucket them and say these are hitting [X] requirement(s) for the *next* level, what do I need for the next level.


Debugging & Avoiding Bugs
----------------------------

Debugging is the process of reconciling your mental model (requirements) of what the code does
with with the code you actually wrote does (artifact)

You need to prioritize things that are likely to fail, and things that are likely to be hard to debug

Don't think of how a feature can be useful, think of how it could go wrong.

Don't make the easy stuff easier (typing/macros), while making the harder stuff harder

 
