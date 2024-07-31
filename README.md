# math-eval

A rust math evaluation library, with a stateful context.

## Rationale

As the time of writing this, I am currently working on a "typing math calculator" where instead of
using a select set of buttons to get a specific result, you can type your whole math expression and
get the result of it.

The issue is, I need a math parser for both of these use cases
- Evaluating the math expressions from user input
- Generate an AST to do syntax highlighting, which is one of the features of my calculator

I already checked existing solutions:
- [`kalk`](https://github.com/PaddiM8/kalker/tree/master/kalk): Written in rust, but I did not want to
wrap my head around yet another library
- [`libqalculate`](https://github.com/Qalculate/libqalculate/): Have fun getting that to work with rust,
since it's a C++ library ([I already tried `cxx-rs`](https://github.com/dtolnay/cxx))
- Other existing rust libraries, but they are all unmaintained, or don't have the feature set I want.

## Current features

Nothing

## TO-DO

- Simple math evaluation using PEMDAS (or however you name them)
- Built-in functions (square-root, cube-root, trig, gcd, etc...)
- Summation and Product notations
- Bit-wise operations
- Variable and function declaration
- Array-wise operations
- Complex numbers
- Calculation of derivatives and integrals
- Support UTF-8/Unicode symbols
- Unit conversions
