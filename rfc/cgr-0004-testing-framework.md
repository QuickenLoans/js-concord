# Testing Framework [Design]

  - Status: proposal
  - Type: Recommendation
  - Start Date: 2017-04-26
  - Discussion: https://github.com/QuickenLoans/js-concord/issues/5
  - Supersedes: none
  - Superseded by: none

## Summary

Define a recommendation for a JavaScript testing framework.

## Conventions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be
interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).

## Motivation

With a variety of JavaScript testing frameworks available, choosing one to
standardize on should assist in knowledge sharing across teams and further the
goal of cross project tool-chain consistency.

# Design

The recommended JavaScript testing framework is [Mocha] for all projects that aren't
using a library or framework that would be better aligned with [Jest].

## Drawbacks

## Alternatives

* [AVA]
* [Jasmine]
* [QUnit]
* [tape]

## Unresolved (questions)

[AVA]: https://github.com/avajs/ava
[Jasmine]: https://jasmine.github.io
[Jest]: https://facebook.github.io/jest/
[Mocha]: http://mochajs.org/
[QUnit]: https://qunitjs.com
[tape]: https://github.com/substack/tape
