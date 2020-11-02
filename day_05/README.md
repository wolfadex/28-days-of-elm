# Day 5 - Records

In our previous days we've worked with people and we've been grouping their name and age in Tuples. Often however we want to be a little more clear about values. Records are a great way to do this! A great example is dealing with coordinates. A Tuple would give us `( 5, 7)`, but which of those is X and which is Y? With a record we have `{ x = 5, y = 7 }`. And if we want to get the values out we can do

```Elm
> point = { x = 5, y = 7 }

> point.x
5
> point.y
7
```

If we want to move our point we can create a new point with a modified X like so

```Elm
> newPoint = { point | x = 10 }

> newPoint.x
10
> point.x
5
```

As you can see, Elm is immutable. This mean we can never change a value. Our original `point` will always be `{ x = 5, y = 7 }` and we have to create a new record to have a point with different values.

Unlike a List, a record doesn't have to have all of the same type of values. So we could creat a record for a person too

```Elm
> carl = { name = "Carl", age = 67, hobby = "Knitting" }
```

## Exercies

1. Write a function that takes a `List person`, where person is a record like `{ name = "Steve", age = 3 }`, and returns the names of people who are below a 5 years old. Those people are eligible for day care.
1. Write a function that takes 2 point records like `{ x = 2, y = 12 }` and adds them together.
1. Write a functoin that takes a record like `{ name = "Square Inc", employees = [ { name = "Stephanie", role = "engineer" }, { name = "Richard", role = "secretary" } ] }` and returns a List of only the engineers.

[Solutions](./SOLUTIONS.md)
