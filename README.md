# BezierMath.js

We are migrating BezierMath.js from Bezier.js implementing mathjs.  The work is just beinning and not yet usable but we expect rapid development with at least the core functions my end of March (2022). The original Bezier.js is still in this repo and will remain until the project has been completely migrated.

In the meantime, for a finished and complete version check out the original at [pomax.github.io/bezierjs](http://pomax.github.io/bezierjs).

An ES Module based library for Node.js and browsers for doing (quadratic and cubic) Bezier curve work.

For a Demo and the API, hit up either [pomax.github.io/bezierjs](http://pomax.github.io/bezierjs) or read the souce (`./src` for the library code, start at `bezier.js`).

## Installation

clone it!  More details later/

### Without using a package manager

There is a rolled-up version of `beziermath.js` or `beziermath,min.js` in the `dist` directory. Just download that and drop it into your module or scipts directory.

## In Node, as dependency

About as simple as it gets:

```
import { BezierMath as bm } from "beziermath";

const b = new bm.Bezier(...);
```

Or, using the legacy CommonJS syntax:

```
const bm = require("beziermath");

const b = new bm.Bezier(...);
```

## In Node or the browser, from file

Copy the contents of the `src` directory to wherever you like (`/js`, `/vendor`, etc), or place the rolled-up version of the library there, and then load the library as an import to whatever script needs to use the `Bezier` constructor using:

```
import { Bezier } from "/js/vendor/bezier.js";

const b = new Bezier(...);
```

## Working on the code

All the code is in the `src` directory, with `beziermath.js` as entry point.

To test code (which automatically applies code formatting and rollup), use `npm test`.

There is no explicit build step for the library, `npm test` takes care of everything, except checking for code coverage.

## License

This code is MIT licensed.

## Engagement

For comments and questions, file an issue.
