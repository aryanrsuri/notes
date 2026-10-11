# Debugging and failure risk

## Reconciling expectations and behavior

Debugging is the process of reconciling your mental model (requirements) of what the code does
with with the code you actually wrote does (artifact)

### Debugging & Avoiding Bugs

Don't make the easy stuff easier (typing/macros), while making the harder stuff harder

## Anticipating failures

!!! One of the most common sources of bugs in a badly architected (lots of moving parts system) is user error.
since bad architecuture makes constraint fails visible and doable by the user.

You need to prioritize things that are likely to fail, and things that are likely to be hard to debug

Don't think of how a feature can be useful, think of how it could go wrong.

## Instrumentation

tags: tech

- Instrument (track, measure & log) everything
- Treat the logs, data, and monitoring as a product --> Inference team

Try to write a test application:

- Minimal
- Logging
- Portable

## Reviewing changes

- PR Reviews
   - On low risk reviews be more high levels and rubber-stamp it
   - On high risk/prod refactors more thorough reviews
   - Defer to how do I accept this diff "what is absolutely blocking this thing from going to prod"
- if you aren't getting negative feedback on pm then keep pushing the $[edge] / boundary of speed
