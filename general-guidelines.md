# General Guidelines

## Architecture and design

- Use Clean Architecture and apply design patterns when possible.
- Try to use BDD (= Behaviour Driven Design) for the design work. 
- Use TDD (test driven development) for the coding phase.

## Object Oriented Development Specific

- Write classes the SOLID way.

## Quality

The first premise on coding should be: **failure is not an option**, a very well known statement within the Ada community. But this starting point should be applied to whatever programming language or platform someone uses to develop software.

Following rules can help:

- Always check incoming parameters. Some form of code contracts or asserts can help if they are available.
- Exceptions must only be used to report issues, **NOT** to return function results.
- Try to avoid the use of primitive types for every kind of data storage. Attempt to encapsulate them in entities or custom value types. For example: if you need a non-zero positive number, create a value type NonZeroInteger which has internal checks whether a proper value is assigned. This way, any asserts on parameters will be far simpler instead of every time checking on each function whether the passed on value is positive and non-zero.

### "Zero-bug" Policy

Although this is not always easy to keep up, it will prove its worth on the long run due to less bugs and more stable software.

- Bugs are fixed first.
- Secondly, mandatory features implemented.
- Then, the removal of technical debt.
- Lastly, the implementation of nice-to-have features.

### Clean coding

- Keep functions small.
- Don't repeat yourself (DRY)
- Each function should do one thing only.
- Avoid side-effects.
- Functions should by preference (and if possible) accept no more than 3 parameters.
