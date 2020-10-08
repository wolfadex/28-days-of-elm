# Solutions - Day 2

Your solutions don't have to look exactly like these. These are just one of many solutions.

1.  ```Elm
    greet name = "Hello " ++ name ++ "!"
    ```
    - Our function takes 1 argument called `name`. It then combines that with the string `"Hello "` and `"!"`
1.  ```Elm
    tax amount = amount * 0.1
    ```
    - We take 1 argument, `amount`, and multiply it by `0.1`
1.  ```Elm
    madLib noun1 noun2 verbed adjective = "The " ++ adjictive ++ " " ++ noun1 ++ ", " ++ verbed ++ " around the green " ++ noun2
    ```
    - We have 4 arguments
        - `noun1` any noun
        - `noun2` any noun
        - `verbed` a verb, preferabbly ending in "ed"
        - `adjective` any adjective
    - We then join them together to tell a story.
