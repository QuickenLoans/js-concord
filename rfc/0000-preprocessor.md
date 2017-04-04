# Preprocessor

  - Status: proposal
  - Type: Recommendation
  - Start Date: 2017-03-03
  - Discussion:
  - Supersedes: none
  - Superseded by: none


## Summary
[Summary]: #summary

Define the recommended JavaScript preprocessor.


## Conventions
[Conventions]: #conventions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be
interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).


## Motivation
[Motivation]: #motivation

The goal is to achieve a consistent code-editing experience across many
projects. A JavaScript preprocessor should work mostly "transparently" to daily
work; it should enable use of newer features but not introduce additional
cognitive overhead. This should promote people contributing to other projects
directly or through "sharing" code.

Choosing a single preprocessor tool/utility will simplify dependency footprint
and enable people to share knowledge or project configuration. Further, this
will enable projects to have a more consistent tool-chain and be built from a
common starting point.


## Design
[Design]: #design

The recommended JavaScript preprocessor is [Babel] for all projects that aren't
using a library or framework that would be better aligned with [TypeScript]. It
is suggested as "best practice" to incorporate a preprocessor - unless some
design aspect of the project specifically conflicts with the use of a
preprocessor - as this will allow for more consistent code editing between
projects.


## Drawbacks
[Drawbacks]: #drawbacks

### Added Complexity

Including a preprocessor, for "compiling" source code into "delivery" code,
increases the complexity of the project; this forces project maintainers and
contributors to understand how to configure and execute the tooling.

The addition of complexity is something that should be evaluated against the
goals of each project; the benefits, that a preprocessor provide, should
"out weigh" the costs before including the preprocessor.

### Wider Dependency Graph

Adding dependencies to a project is not something that should be trivialized or
ignored at any stage of a project's development. As the dependency graph of a
code-base grows so to does the difficulty of keeping all dependencies
"up-to-date".


## Alternatives
[Alternatives]: #alternatives

There is a subtle distinction between [Preprocessors] and [Transpilers].

### Preprocessors
[Preprocessors]: #preprocessors

Preprocessors focus on compiling JavaScript to JavaScript; the source language
is JavaScript.

  - [Traceur](https://github.com/google/traceur-compiler)
  - [Closure Compiler](https://developers.google.com/closure/compiler/)
  - [Esprima](http://esprima.org/)


### Transpilers
[Transpilers]: #transpilers

Also known as "compile-to-js" languages because the source language is very
much not JavaScript; typically an established language in its own right.

  - [CoffeeScript](http://coffeescript.org/)
  - [LiveScript](http://livescript.net/)
  - [PureScript](http://www.purescript.org/)
  - [Elm](http://elm-lang.org/)


## Unresolved (questions)
[Unresolved]: #unresolved-questions

<!--
What parts of the design are still to be done?
-->


[Babel]: http://babeljs.io/
[TypeScript]: https://www.typescriptlang.org/
