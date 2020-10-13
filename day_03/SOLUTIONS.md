# Solutions - Day 3

Your solutions don't have to look exactly like these. These are just one of many solutions.

1.  ```Elm
    canVote age = if age >= 18 then "You can vote!" else "You have to wait to vote."
    ```
    - Our function takes 1 argument called `age`. It then checks that the age is at least 18 (voting age in the US).
1.  ```Elm
    evenOrOdd num = if modBy 2 num == 0 then "even" else "odd"
    ```
    - We take 1 argument, `num`, and modular divide by 2. If the result is 0 then the number is even.
1.  ```Elm
    checkPassword password = if password == "peanutbutter" then "Welcome friend!" else "You are not welcome here."
    ```
    - We take 1 argument, `password`, and compare it against the secret password.
