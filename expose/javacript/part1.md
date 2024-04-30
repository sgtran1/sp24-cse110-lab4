
## var declaration 
1. Line 9 contains a `console.log` statement inside the `if` block. It prints the result of adding `num1` and `num2` together. So, if the code runs without any errors and `sumValues(10, 10, true)` is called, line 9 will print: "values added: 20".
2. Line 13 contains another `console.log` statement attempting to print the final result outside of the `if` block. However, even though `result` is declared inside the `if` block, it is accessible outside of that block but inside the function. It will print: "final result: 20"

## let declaration
3. Line 9: It would print "values added: 20" if the code runs without any errors and sumValues(10, 10, true) is called. This is because result would be correctly scoped within the if block due to the usage of let.
4. Line 13: It would result in a ReferenceError. This is because result would only be accessible within the if block due to the usage of let. Attempting to access result outside of the if block would result in an error.

## const declaration
5. Line 9: It would print "values added: 0" if the code runs without any errors and sumValues(10, 10, true) is called. This is because with const, result cannot be reassigned after its initial assignment of 0. So, even though result is initialized to 0, it cannot be updated to reflect the sum of num1 and num2.
6. Line 13: It would still result in a ReferenceError for the same reason as before. result would only be accessible within the if block due to the usage of const, and attempting to access result outside of the if block would result in an error

## 




