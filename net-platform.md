# .NET Platform

## Naming and Coding Conventions

- Use Microsoft naming conventions and formatting of C#, unless there is a good reason to deviate from it. Those deviations must be documented in these guidelines.
- Although C# is not a functional programming language, it has some features that can be used to write code is such a style. Therefor, the advise is to apply such a FP coding style in C#.

## Implementation guidelines

- Entity classes should implement at least the following overrides: *ToString()*, *Equals()*, *GetHashCode()*. This functions will not only be useful for normal use but also during testing.
- Use interfaces above classes as types to improve code-reuse.

## NuGet packages

A specific, basic set of NuGet packages will be used. The selection of those packages will allow for faster development times by avoiding the need to constantly look for libraries to do re-occurring work, the decisions about which packages to use are already made.

It is definitly not required but keeping a copy of the library code might be useful to consider in case a library maintainer suddenly decides to remove the library on which any current projects are depending on.

Selected packages:

- [Command line parsing](https://github.com/commandlineparser/commandline)

## References

[Microsoft C# Coding Conventions](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)