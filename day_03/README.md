# Day 3 - Conditionals & Tuples

So far we learned how to create values and how to modify them. Next up we'll learn how to conditionally return different values and how to work with something called a tuple.

### Conditionals

Conditionals are means of returning different values in your code. What this looks like in Elm is called an if expression.

```Elm
result =
    if condition then
        value1
    else
        value2
```

What this is saying is that if `condition` is `True` then we set `result` to `value1`, otherwise we set `result` to `value2`. A more detailed example of this could look like a function to check the age of a user and see if they qualify for something. This might look like

```Elm
canDrink age =
    if age >= 21 then
        "Can drink in the US."
    else
        "Cannot drink in the US."
```

You may also notice that both branches if the if express, the part after `then` and after `else` are both strings. That is, no matter the condition the if expression must return the same type of value.

### Tuples

Tuples are means of grouping data

## Exercies

1. TODO

[Solutions](./SOLUTIONS.md)
