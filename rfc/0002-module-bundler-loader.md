# Module bundler/loader

  - Status: proposal
  - Type: Recommendation
  - Start Date: 2017-03-08
  - Discussion:
  - Supersedes: none
  - Superseded by: none


## Summary
[Summary]: #summary

Define a recommendation for a JavaScript module bundler or loader.


## Conventions
[Conventions]: #conventions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be
interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).


## Motivation
[Motivation]: #motivation

Until support for native module loading is widely available, a separate bundling
or loading tool is necessary to make effective use of JavaScript modules. The goal
of this standard is to recommend one tool so projects can implement modules in a
consistent way. This will enable more knowledge sharing and will make it easier for
developers to switch between projects.


## Design
[Design]: #design

It's suggested as a "best practice" for projects to incorporate a JavaScript bundler and the recommended bundler is [Webpack](https://webpack.js.org/).

Additionally, these are some recommended Webpack loaders that will help with standards compliance:

  - [Babel Loader](https://github.com/babel/babel-loader)
  - [ES Lint Loader](https://github.com/MoOx/eslint-loader)


## Drawbacks
[Drawbacks]: #drawbacks

  - **Complexity** - A bundler, like Webpack, necessitates a project build step. Because of this, projects will have more dependencies, more documentation/coaching will be required to get new developers up and running, and there will be more points of failure.
  - **Learning Curve** - Because Webpack has a lot of features, it can take time to fully understand the options available and whether they're applicable to a given project or not.


## Alternatives
[Alternatives]: #alternatives

  - [Rollup](https://rollupjs.org/)
  - [Browserify](http://browserify.org/)


## Unresolved (questions)
[Unresolved]: #unresolved-questions
