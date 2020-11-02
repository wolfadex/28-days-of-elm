# Solutions - Day 4

1.  ```Elm
    product nums = List.foldl (\num total -> num * total) 1 nums
    ```
    - Like using `List.foldl` for adding everything together, here we multiply.
    - Note that the starting value is `1` because 1 times any thing is always that thing.
1.  ```Elm
    aboveN min nums = List.filter (\num -> num > min) nums
    ```
    - `List.filter` takes a function that returns `True` or `False`.
1.  ```Elm
    dayCareEligible people =
        List.foldl
            (\( name, age ) result ->
                if age < 5 then
                    name :: result

                else
                    result
            )
            []
            people
    ```

    - We start out with an empty list because we don't have anyone below 5 years old.
    - If they're below 5, then we put that name on the front of our resulting List.
    - If they're 5 or older we return the current List.
