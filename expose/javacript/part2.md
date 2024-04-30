1. At line 12, the console.log(i); statement will print the value of i. In this case it will print out "3". The variable i was initialized as a var. So, after the loop finishes executing, i will hold the value of prices.length, because that's the condition under which the loop terminates. Therefore, console.log(i); will print the length of the prices array. 
2.  attempting to print discountedPrice outside of the loop will print 150 which is the dicount price of last item. Since it was declared var it can be referecne in function so no error
3.  attempting to print final outside of the loop will print 150 which is the final price of last item. Since it was declared var it can be referecne in function so no error
4.  The variable discounted is an array that stores the discounted prices calculated within the discountPrices function. In the function, during each iteration of the loop over the prices array, a discounted price is calculated using the formula prices[i] * (1 - discount). This discounted price is then rounded to two decimal places using Math.round(discountedPrice * 100) / 100, and pushed into the discounted array using discounted.push(finalPrice). So, by the end of the loop, discounted array contains all the discounted prices calculated for each item in the prices array. Finally, the function returns this discounted array.
5. At line 12, an error will occur because i is not accessible outside the scope of the for loop. In JavaScript, variables declared with let have block scope, meaning they are only accessible within the block they are declared in. In this case, i is declared within the for loop, so it's only accessible within that loop. When the console.log(i); statement is executed outside the loop, there's no variable i defined in that scope, resulting in a ReferenceError
6. At line 13, a ReferenceError will occur because discountedPrice is declared within the for loop block, and therefore it is only accessible within that block. In JavaScript, variables declared with let have block scope, meaning they are limited to the block in which they are defined. In this case, discountedPrice is declared inside the for loop, so it is only accessible within that loop. When the console.log(discountedPrice); statement is executed outside the loop, there's no variable discountedPrice defined in that scope, resulting in a ReferenceError.
7. At line 14, the console.log(finalPrice); statement will output the last calculated finalPrice for the last item in the prices array. This will not cause an error because finalPrice is declared outside the loop and is accessible within the entire discountPrices function since they are in the same block. The variable finalPrice is being updated in each iteration of the loop, and finally, the last updated value is logged to the console before the function returns.
8. The variable discounted is an array that stores the discounted prices calculated within the discountPrices function. It was declared using let keyword In the function, during each iteration of the loop over the prices array, a discounted price is calculated using the formula prices[i] * (1 - discount). This discounted price is then rounded to two decimal places using Math.round(discountedPrice * 100) / 100, and pushed into the discounted array using discounted.push(finalPrice). So, by the end of the loop, discounted array contains all the discounted prices calculated for each item in the prices array. Finally, the function returns this discounted array.
9. At line 11, an error will occur because you're trying to reassign a value to a constant variable finalPrice
10. At line 12, console.log(length) will output the length of the prices array, which is stored in the variable length. This code will not cause an error. length is a variable declared within the function scope, storing the length of the prices array. Since it's properly defined and accessed within the function, console.log(length) will output the length of the prices array, which is 3.
11. The function will return an array containing the discounted prices of the items in the prices array. It won't cause an error because all variables are properly scoped and used within the function.
12. 
// Accessing the value of the name property in the student object
student.name

// Accessing the value of the Grad Year property in the student object
student['Grad Year']

// Calling the function for the greeting property in the student object
student.greeting()

// Accessing the name property of the object in the Favorite Teacher property in student
student['Favorite Teacher'].name

// Accessing index zero in the array of the courseLoad property of the student object
student.courseLoad[0]
13. 
A. '3' + 2

Output: '32'
Explanation: JavaScript performs concatenation instead of addition because one operand is a string. The number 2 is coerced into a string and concatenated with '3'.
B. '3' - 2

Output: 1
Explanation: JavaScript performs subtraction. The string '3' is converted into a number, resulting in 3 - 2 = 1.
C. 3 + null

Output: 3
Explanation: The null value is coerced into a number, which is 0 in numeric context. So, 3 + 0 = 3.
D. '3' + null

Output: '3null'
Explanation: Similar to the first case, JavaScript performs concatenation. The null value is coerced into the string 'null' and concatenated with '3'.
E. true + 3

Output: 4
Explanation: The boolean value true is coerced into the number 1, so 1 + 3 = 4.
F. false + null

Output: 0
Explanation: Both false and null are coerced into the number 0, so 0 + 0 = 0.
G. '3' + undefined

Output: '3undefined'
Explanation: Similar to the fourth case, JavaScript performs concatenation. The undefined value is coerced into the string 'undefined' and concatenated with '3'.
H. '3' - undefined

Output: NaN (Not a Number)
Explanation: JavaScript tries to perform subtraction, but since undefined cannot be coerced into a number, it results in NaN.

14. 
A. '2' > 1

Output: true
Explanation: JavaScript performs type coercion when comparing values of different types. The string '2' is converted into a number, resulting in 2 > 1, which evaluates to true.
B. '2' < '12'

Output: false
Explanation: JavaScript compares strings character by character. Since '2' is lexicographically greater than '1', '2' is also greater than '12', resulting in false.
C. 2 == '2'

Output: true
Explanation: JavaScript performs type coercion for equality comparisons. The string '2' is coerced into the number 2, so 2 == 2, which evaluates to true.
D. 2 === '2'

Output: false
Explanation: The strict equality operator (===) does not perform type coercion. Since 2 is a number and '2' is a string, they are of different types, resulting in false.
E. true == 2

Output: true
Explanation: JavaScript performs type coercion for equality comparisons. The boolean true is coerced into the number 1, so 1 == 2, which evaluates to false.
F. true === Boolean(2)

Output: false
Explanation: The strict equality operator (===) does not perform type coercion. Here, Boolean(2) evaluates to true, but since true and Boolean(2) are of different types (boolean and boolean), the result is false.

15. 
The == operator in JavaScript checks for equality after attempting type coercion, converting operands to the same type before comparison. This can lead to unexpected results when comparing values of different types. In contrast, the === operator strictly compares both the value and the type of the operands, without performing any type coercion, providing more predictable behavior.

16. In part2-question16.js file 
    
17. Calling modifyArray([1, 2, 3], doSomething) will return [2, 4, 6]. This result is obtained by iterating through each element of the input array, applying the doSomething function (which doubles each element), and storing the results in a new array, which is then returned.
    
18. In part2-question18.js file 
19. The output is 
1
4
3
2

The printNums function logs the numbers 1 and 4 synchronously, while asynchronously logging the numbers 2 and 3 after 1 second and immediately (due to the minimum delay being set to 0 milliseconds), respectively, upon its invocation.

20. 


