# JavaScript Loose Comparison Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to loose comparison (==) with NaN and +0/-0.  Loose comparison doesn't always behave as one might intuitively expect.

The `bug.js` file shows the problematic code.  The `bugSolution.js` file provides a solution.

## Problem

JavaScript's loose comparison operator (==) considers NaN to not be equal to itself, and +0 to be equal to -0. This behavior can result in unexpected outcomes.  Strict comparison (===) solves the NaN issue, but still leaves the +0/-0 ambiguity.