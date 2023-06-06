# HaskHell

# 1. INTRODUCTION

## What is functional programming ?

Functions are a combinations of _expressions_. Expressions include concrete values, variables, functions. 
Functions: Expressions that are applied to an argument / input and can be reduced or evaluated. Functions can be used as values or passed as arguments, or inputs, more functions. 

## What is a Function (Math)
You can see it as a mapping of set of inputs to a set of outputs.
![image](https://github.com/jonathancastro21/haskhell/assets/131474704/f263b18d-90fa-42bd-ad2e-9a6123697d7e)

This is **not** a valid function ? 
![image](https://github.com/jonathancastro21/haskhell/assets/131474704/3cee2859-0697-4af1-b405-12a4dcd57b3c)

## What are lambda terms ?
![image](https://github.com/jonathancastro21/haskhell/assets/131474704/df65293b-c348-44cb-86bb-fa310d4a26cb)

## What is a lambda abstraction ?
A lambda abstraction is an anonymous function or lambda term. 

** The meaning of Haskell programs is centered around evaluating expressions ** 

# 2. BASIC EXPRESSIONS AND FUNCTIONS

## What are Expressions ?

Expressions may be values, combinations of values and/or functions applied to values.

- Normal Form: Expressions are in Normal form when they have reached an **irreducible** form
- Redex: Reducible expressions

## What are functions ?

Functions are a specific type of expression that is applied to an argument. They Map an input or set of inputs to an output. 

- Currying: It seems that we are passing multiple arguments to a function, we are actually applying a series of a nested functions, each to one argument.

### How do you define Functions ? 

1. Start with the name of the function
2. Followed by the formal parameters (/=Argument)
3. Equal sign which expresses the equality of the terms
4. Expression which is the body of the function and can be evaluated to return a value

triple x   =  x * 3

**Capitalization matters!** 
Function -> camelCase Style
Variables -> lowercase Style

## Evaluation

What does "Evaluating an Expression" mean ? : Reducing the terms until the expression reaches its simplest form

How do you evaluate ?: Haskell uses a nonstrict evaluation (lazy evaluation) which defers ("verschieben") evaluation of terms until they are forced by other terms referring to them.

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

# 3. STRINGS

# 4. BASIC DATATYPES
- Learn about Datatypes, Type constructors, data constructors
- Work with predefined Datatypes
- Type signatures and a bit about type-classes

What are types ? : Types are how we group a set of values together that share something in common.
Data declarations: How Datatypes are defined. 
Type Constructor: name of the type and is capitalized
Data Constructor: Values that inhabit the type they are defined in. The values that show up in your code. 

Data Declaration: 
![image](https://github.com/jonathancastro21/haskhell/assets/131474704/6e032468-2ccc-4110-bf7f-918adb175974)

## Numeric Types

- Integral numbers: These are whole numbers, positive and negative.
  - `Int`: Fixed-precision integer. It has a range, with a maximum and a
minimum
  -  `Integer`:  This type is also for integers, but this one supports arbitrarily large (or small) numbers.
-  Fractional: These are not integers. Fractional values include the following four types:
  - Float: This is the type used for single-precision floating point numbers.
  - Double: This is a double-precision floating point number type.
  - Rational:This is a fractional number that represents a ratio of two integers. The value 1 / 2 :: Rational will be a value carrying two Integer values, the numerator 1 and the denominator 2, and represents a ratio of 1 to 2. Rational is arbitrarily precise but not as efficient as Scientific.
  - Scientific:  This is a space efficient and almost arbitrary precision scientific number type. Scientific numbers are represented using scientific notation. It stores the coefficient as an Integer and the exponent as an Int.

Which numeric datatype all those instances have ?: Typeclass `Num`
What are typeclasses ? : A way of adding functionality to types that are reusable across all the types that have instances of that typeclass. 

## Boolean
_coming soon.._

## Tuples
_coming soon.._

## Lists
_coming soon.._

# 5. TYPES
- Learn about querying and reading type signatures
- take a closer look at different kinds of polymorphism
- look at type inference and how to declare types for our functions

















































