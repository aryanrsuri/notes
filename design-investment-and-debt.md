# Design investment and debt

## Investing in future development

> Write code so it never breaks

> Its faster to write `N` lines of code today,
> Than write `k << N` lines of code today, and edit later.

### Can Great Programmers Be Taught?

https://youtu.be/LtRWu9DErgU?si=7yebqitDhwwxJMFy

- There exists `Strategies` versus `Tactical` programming

#### Tactical

- Get next feature/bug-fix working
- A few shortcuts and kludges are **OK**
- Result --> Bad design with high complexity
- Complexity is Incremental, death by one-thousand cuts
- Extreme: Tactical Tornadoes (Literally Me)
   - Can ship extremely fast, get the next feature or bug-fix done, land the PR
   - The problem is they get things 80% done, use shortcuts, slop, or kludges, and leave a mess of debt
- Most startups are tactical, and `clean later`, but code becomes spaghetti. Facebook is a great example
   - Move quickly and break things
   - eventually realised
   - Move quickly with solid infrastructure

#### Strategic

- Produce a great design
- Simplify future development
- Minimise complexity, "sweat the small stuff"
- Investment mindset: Take more time now, pay back later

#### How much to Invest?

- Make continual small improvements, ~20% overhead
- When writing new code:
   - Careful design
   - Good documentation
- When changing new code:
   - After change, system is the way it *would* have been designed if that way from the start
   - Always find something to improve
- Ask yourself: Is this the most I can afford to invest right now?

## The cost of change

https://martinfowler.com/bliki/TechnicalDebt.html

https://youtu.be/ukgmp6uxQJc?si=B-NwkKLqhFw4ECvd

https://sites.google.com/site/unclebobconsultingllc/a-mess-is-not-a-technical-debt

> software systems are prone to the build up of **cruft**
> -deficiencies in internal quality that make it harder than
> it would ideally by to modify and extend the system further.
> Martin Fowler

Ultimately it is a tradeoff, but the best is if there are
high cruft, high stable areas of the codebase you can avoid
paying this debt. Conversly, high-churn parts of the codebase
we should **abjure** the presence of debt.

Uncle Bob argues that

> A mess is not a debt
> -* Uncle Bob

> i.e that bad code (produced by lack of good sofwtare design)
> isn't a *debt* but a loss-a mess. Technical debt (in Bob's POV)
> should be concious decisions based on project constraints, and
> risky. Messes are *not* rational, as debt should be.

> **Fowler's Response**

> Not exaclty, technial debt is a metaphor, and thus it is not about
> whether a flaw is debt *or not*, but wether the metaphor is helpful.
> Messy code *is* a debt, but reckless and bad.

It's often the case that it can take a year of programming on a project
before you understand what the best design approach should have been.

Thus, it becomes a x-y graph

```text
                Deliberate
                   |
-x(Reckless)-------|-------(Prudent)+x
                   |
                Inadvertent

-x+y (We don't have time for design)
-x-y (What's layering?)
+x+y (We must ship now and deal with the consequences)
+x-y (Now we know how we should have done it)
```

![](https://martinfowler.com/bliki/images/design-stamina-hypothesis/graph.png)

## Discardable first versions

### Cathedral and the Bazaar

1. Plan to throw one [version] away; you will, anyhow
   (copied from Frederick Brooks's _[The Mythical Man-Month](https://en.wikipedia.org/wiki/The_Mythical_Man-Month "The Mythical Man-Month")_).
