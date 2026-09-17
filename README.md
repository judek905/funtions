# JS Practice: Functions & DOM Basics

A small sandbox for practicing JavaScript fundamentals — function declarations, expressions, arrow functions, and hooking JS up to an HTML page.

## What's in here

- **`index.html`** — A bare-bones page with two buttons. One fires an inline `alert()`, the other calls a function defined in an external script.
- **`external.js`** — A tiny external script with a `greet()` function, linked into `index.html` to show how external JS files work.
- **`functions.js`** — A set of examples covering different ways to write functions in JS:
  - Function declarations vs. function expressions vs. arrow functions
  - Simple math helpers (`add`, `multiply`)
  - A few "real world" examples: greeting a user, depositing money, withdrawing money (with a basic insufficient-funds check)

## How to run it

Just open `index.html` in a browser. Click the buttons to see the alerts fire.

To play with `functions.js` on its own, open it in a browser console or run it with Node:

```bash
```

## Heads up — known issues

This file is a work in progress and currently has a couple of bugs worth knowing about:

- `multiply(a, b)` is declared with no parameters but tries to use `a` and `b` anyway — it needs parameters added.
- `add` is defined twice (once as a `const` function expression, once as a `function` declaration). JavaScript won't allow both in the same scope — pick one.
- `console.log(add(5,6))` is called before `add` is defined further down the file, which will throw an error in the `const` version.

Good next step: fix these, then rerun to confirm each example logs the expected output.

## Why this exists

Practice repo for getting comfortable with core JS syntax before moving on to more advanced topics (this pairs well with the JS/React additions being made to the Marlow & Rye bakery site).
