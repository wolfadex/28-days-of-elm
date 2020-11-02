# Solutions - Day 5

1.  ```Elm
    dayCareEligible people =
        List.foldl
            (\person result ->
                if person.age < 5 then
                    person.name :: result

                else
                    result
            )
            []
            people
    ```

    - Like the solution in Day 4 except with a record.

1.  ```Elm
    addPoints point1 point2 =
        { x = point1.x + point2.x
        , y = point1.y + point2.y
        }
    ```

    - You could also add them like `{ point1 | x = point1.x + point2.x, y = point1.y + point2.y }`.

1.  ```Elm
    getEngineers company =
        List.filter
            (\employee -> employee.role == "engineer")
            company.employees
    ```

    - Once we learn future things like pattern matching and Types we can make this solution a lot better.
