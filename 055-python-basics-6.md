# 55 - Python Basics 6

*Written by Emily Leng*

## Problem

Given an integer value stored in `args[0]`, find the sum of all numbers less than or equal to `args[0]` and greater than zero that are divisible by 7. Then, print the sum of all the digits of the original sum to get your answer.

## Hint

What is a math operation to check divisibility?

## Solution

```python
tmp = 0
for i in range(7, args[0]):
    if i % 7 == 0:
        tmp += i

digits = 0
while tmp:
    digits += tmp % 10
    tmp /= 10

print digits
```

## Flag

`beginner_math_loops_5_e_z_3_me`
