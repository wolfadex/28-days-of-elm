# Day 4 - Lists

### List Basics

When programming we often need a way to group many values. This is usually refered to as a data structure. In Elm Lists are one of the most common data structures. A List is a sequential grouping of similar values. For example a list of numbers would look like `[ 4, 19, 700, 52, 10 ]` and a List of strings like `[ "Wolfgang", "Alice", "Carey" ]`.

We can also use List specific functions to get information about our List. Some examples are:

```Elm
> List.length [ 4, 19, 700, 52, 10 ]
5

> List.isEmpty [ 4, 19, 700, 52, 10 ]
False

> List.sort [ "Wolfgang", "Alice", "Carey" ]
[ "Alice", "Carey", "Wolfgang" ]

> List.reverse [ "Alice", "Carey", "Wolfgang" ]
[ "Wolfgang", "Carey", "Alice" ]
```

If you want to exlpore all of the List functions you can check out the docs here https://package.elm-lang.org/packages/elm/core/latest/List.

Because Elm is all about values and functions, there are a lot of functions that take functions as arguments. A great example of this with Elm is `List.map`. This function allows us to iterrate over each item in our List and modify it. First we'll make a function called `increment` that adds 1 to a number. Then we'll map over our List of number to increment every number.

```Elm
> increment num = num + 1

> List.map increment [ 1, 2, 3 ]
[ 2, 3, 4 ]
```

We can also write the increment function inline using an anonymous function like so

```Elm
> List.map (\num -> num + 1) [ 1, 2, 3 ]
[ 2, 3, 4 ]
```

### Common List Functions

Other than `List.map`, a few other popular List functions are `::` and `List.foldl`. That first one is called "cons" and is used to add an item to the front of a List like so

```Elm
> 5 :: [ 12, 60 ]
[ 5, 12, 60 ]
```

`List.foldl` on the other hand is like `List.map` in that it's used for iterrating over a List but it's used for creating new values or data structures. A simple use case for `List.foldl` is to sum up all values of a List:

```Elm
> List.foldl (\num total -> total + num) 0 [ 1, 2, 3, 4 ]
10
```

The second argument to `List.foldl` is the starting value.

## Exercies

1. Write a function that calculates the product of a list of numbers.
1. Write a function that filters a List by numbers grater than 22.
1. Write a function that takes a `List ( String, Int )`, where the `String` is a name and the `number` is and age, and returns the names of people who are below a 5 years old. Those people are eligible for day care.

[Solutions](./SOLUTIONS.md)
