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

Tuples are means of grouping together a small number of values. A basic example would be `( "Kyle", 36 )`. This can be quite useful if you wanted to return both a name and age from a function. You can even group together 3 values into a tuple like so `( value1, value2, value3 )`, however that's the most you can put into a tuple. It is not advised to use tuples for thing like coordinates though. If you were to see `( 5, 18 )` would you know which of those is the X coordinate and which is the Y? You might have a good guess but you don't know for certain.

## Exercies

1. Write a function that takes an age and returns a string saying whether or not the person can legaly vote.
1. Write a function that takes a number and returns a string saying if the number is even or odd.
1. Write a function that takes checks a password and returns a corresponding response.

[Solutions](./SOLUTIONS.md)
