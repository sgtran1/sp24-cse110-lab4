1. What was the bug?
The bug in the code is that num1 and num2 are retrieved from the HTML inputs as strings, not numbers. When you use the + operator with strings, it concatenates them rather than adding them mathematically.

2. How would you fix it? Include a screenshot of your fix. Name it fix.png (or whatever image extension you would like to use) and add it to your expand/screenshots directory.
To fix this, you need to convert num1 and num2 to numbers before performing addition. You can use the parseInt() function to convert them to integers: