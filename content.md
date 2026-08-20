# What Is an Accumulator?

An accumulator is a variable that stores an ongoing result while a loop runs.
Each iteration updates the accumulator using the current item, so the result builds up step by step.

# General Pattern

```
result = initial_value
FOR each item IN iterable:
    result = update(result, item)
OUTPUT result
```

# Choosing the Initial Value

Depending on the operation you're performing, the initial value of the accumulator will differ. Here are some common choices:

* Use `0` when accumulating a sum.
* Use `1` when accumulating a product.
* Use an empty string when building text.
* Use an empty list when building a list.

# Example in Pseudocode

To sum a list of numbers:

```
total = 0
FOR each number IN numbers:
    total = total + number
```

The accumulator `total` starts at 0 and is increased by each number in the list as that number is processed in the for loop.
