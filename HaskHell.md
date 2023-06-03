# HaskHell

# 1. INTRODUCTION

## What is functional programming ?

Functions are a combinations of _expressions_. Expressions include concrete values, variables, functions. 
Functions: Expressions that are applied to an argument / input and can be reduced or evaluated. Functions can be used as values or passed as arguments, or inputs, more functions. 

## What is a Function (Math)
You can see it as a mapping of set of inputs to a set of outputs.

** The meaning of Haskell programs is centered around evaluating expressions ** 

# 2. BASIC EXPRESSIONS AND FUNCTIONS

## Understanding expressions

Expressions may be values, combinations of values and/or functions applied to values.

- Normal Form: Expressions are in Normal form when they have reached an **irreducible** form
- Redex: Reducible expressions

## Functions

Functions are a specific type of expression that is applied to an argument. They Map an input or set of inputs to an output. 

- Currying: It seems that we are passing multiple arguments to a function, we are actually applying a series of a nested functions, each to one argument.

### Defining Functions 

1. Start with the name of the function
2. Followed by the formal parameters (/=Argument)
3. Equal sign which expresses the equality of the terms
4. Expression which is the body of the function and can be evaluated to return a value

triple x   =  x * 3

**Capitalization matters!** 
Function -> camelCase Style
Variables -> lowercase Style

## Evaluation

Evaluating an Expression: Reducing the terms until the expression reaches its simplest form

Haskell uses a nonstrict evaluation (lazy evaluation) which defers ("verschieben") evaluation of terms until they are forced by other terms referring to them.

Haskell evaluates to weak head normal form (WHNF) by default, which means that not everything will get reduced to its irreducible form immediately.

## Infix Operators

### Associativity and precedence

## Declaring values

### Troubleshooting

The indentation of Haskell code is significant and can change the meaning of the code. Indentation replaces syntatic markers 
like curly brackets, semicolons and parentheses. 

**Use spaces, not tabs, to indent your source code.**

Code that is part of an expression should be indented under the beginning of that expression. Party of 
the expressions that are grouped should be indented to the same level.

`code/learningFile.hs: 10: 1` That indicates that the mistake is in line 10, column 1 of the named file.

## Arithmetic Functions in Haskell

![image](https://github.com/jonathancastro21/haskhell/assets/131474704/f64eebb2-bca6-4923-9bca-f950dd23642f)

- `mod` and `rem` can only represent intregal division
- If you want to divide a smaller number by a larger number and return a fractional answer: `/`

## Let and where

- Let introduces a expression.
- Where is a declaration and is bound to a sorrounding syntatic construct.
- Scope: Area of source code where a binding of a variable applies.

# 3. SIMPLE OPERATIONS WITH TEXT

## Printing strings








































