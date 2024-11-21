---
layout: page
title: Python
description: >-
    Python Reference Guide
nav_order: 5
---

# Python Reference

{:.no_toc}
Created by Brandon Concepcion
{: .no_toc .text-delta }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

### Data Types 


| **Data Type**      | **Description**                                             | **Examples**               |
|--------------------|-------------------------------------------------------------|---------------------------------|
| `int`              | Represents integers: whole numbers that are positive or negative.             | `42`, `-100`, `0`               | 
| `float`            | Represents decimal numbers (floating-point).                | `3.14`, `-1.23`, `0.0`          | 
| `str`              | Represents text (strings of characters).                    | `"Hello"`, `'Data'`             |
| `bool`             | Represents boolean values (`True` or `False`).              | `True`, `False`                 |

### Arithmetic Operators 

| **Numeric Expression**  | **Description**                                                                 | **Examples**                           |
|-------------------------|---------------------------------------------------------------------------------|----------------------------------------|
| **Addition (`+`)**       | Adds two numbers together.                                                       | `2 + 3` would return `5` <br><br> `x + 10` adds `10` to the value of `x` |
| **Subtraction (`-`)**    | Subtracts the second number from the first.                                      | `5 - 2` would return `3` <br><br> `x - 4` subtracts `4` from `x` |
| **Multiplication (`*`)** | Multiplies two numbers.                                                          | `3 * 4` would return `12` <br><br> `x * 2` multiplies `x` by `2` |
| **Division (`/`)**       | Divides the first number by the second, returns a floating-point result.         | `10 / 2` would return `5.0` <br><br> `x / 4` divides `x` by `4` |
| **Floor Division (`//`)**| Divides the first number by the second, rounds down to the nearest integer.       | `10 // 3` would return `3` <br><br> `x // 2` divides `x` and rounds down |
| **Modulus (`%`)**        | Returns the remainder of dividing the first number by the second.                | `10 % 3` would return `1` <br><br> `x % 2` checks if `x` is even or odd (remainder) |
| **Exponentiation (`**`)**| Raises the first number to the power of the second number.                       | `2 ** 3` would return `8` <br><br> `x ** 2` squares `x` |
| **Unary Negation (`-`)** | Returns the negative of the number.                                              | `-x` returns the negative of `x` <br><br> `-10` would return `-10` |



### Variables and Expressions

| **Concept**           | **Description**                                                                 | **Examples**                           |
|-----------------------|---------------------------------------------------------------------------------|----------------------------------------|
| **Expression**        | Any combination of values, variables, operators, and function calls that evaluates to a value. | `2 + 3`, `x * 10`, `len('hello')`     |
| **Variable**          | A name that refers to a value or an expression result. Can be reassigned to different values.  | `x = 10` <br><br> `name = "Sid"`          |
| **Assignment**        | The process of assigning a value to a variable using the `=` operator.                     | `age = 25` assigns the value of 25 to the variable `age` <br><br> `total = price * quantity` sets the `total` variable equal to the product of the values in the `price` and `quantity` variable|
| **Arithmetic Expression** | An expression involving arithmetic operators (`+`, `-`, `*`, `/`, `%`, `**`, `//`).      | `a + b`, `3 * 4`, `10 / 2`, `2 ** 3`  |
| **Comparison Expression** | An expression that compares two values using operators (`==`, `!=`, `>`, `<`, `>=`, `<=`), and returns either `True` or `False`| `a == b` check the equivalency of a and b <br><br> `5 > 3` will return `True` <br><br> `x != y` checks if `x` is **not** equal to `y`, returning `True` if it is not<br><br>            |
| **String Expression**  | An expression that manipulates strings with operators like `+` for concatenation or `*` for repetition. | `"Hello" + " World"`, `"a" * 3`  |
| **Variable Reference** | Referring to a variable in an expression to use its value.                                   | `x * 5` would return the value of `x` times 5 <br><br> `count - 1` would return the value of `count` minus 1  |
| **Compound Expression**| A combination of multiple expressions into one, possibly using parentheses for grouping.     | `(a + b) * 3`         |


