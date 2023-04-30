### Part 2 ###

1. Line 12 prints "3". Since `i` is defined as a `var`, it can be accessed anywhere inside the function it is defined. So when line 12 tries to get `i`, it gets "3", that `i` is assgined while processing `for` loop for the last time. 
2. Line 13 prints "150". Since `discountedPrice` is defined as a `var`, it can be accessed anywhere inside the function it is defined. And the latest assignment of `discountedPrice` is when `i = 3` and `discountedPrice = prices[3] * (1 - 0.5)`, that `discountedPrice` = 300*(0.5) = 150. 
3. Line 14 prints "150". Since `finalPrice` is defined as a `var`, it can be accessed anywhere inside the function it is defined. And the latest assignment of `finalPrice` is when `i = 3` and `finalPrice = Math.round(150 * 100) / 100`, that `finalPrice` = 150. 
4. Nothing is printed, since none of the lines calls the funtion `console.log()`. This function returns `discounted`, and it should be `[ 50, 100, 150 ]`, since discounted[0] = (100 * 0.5), discounted[1] = (200 * 0.5), and discounted[2] = (300 * 0.5).
5. The code returns an error: "ReferenceError: i is not defined". It is because `i` is defined inside the `for(...){...}` block, and `let` provides block scope, which means that `i` cannot be accessed from outside the block at line 12. 
6. The code returns an error: "ReferenceError: discountedPrice is not defined". It is because `discountedPrice` is defined inside the `for(...){...}` block, and `let` provides block scope, which means that `discountedPrice` cannot be accessed from outside the block at line 13. 
7. The code returns `150`. This is because `finalPrice` is defined in the same block that `console.log(finalPrice);` is called. And the last assignment of `finalPrice` is (300 * 0.5), which is 150. Note that variables with `let` could be reassigned in another block inside the block it is declared. 
8. Nothing is printed, since none of the lines calls the funtion `console.log()`. This function returns `discounted`, and it should be `[ 50, 100, 150 ]`, since discounted[0] = (100 * 0.5), discounted[1] = (200 * 0.5), and discounted[2] = (300 * 0.5). 
9. The code returns an error: "ReferenceError: i is not defined". It is because `i` is defined inside the `for(...){...}` block, and `let` provides block scope, which means that `i` cannot be accessed from outside the block at line 11. 
10. The code returns `3`. This is because `length` is defined in the same block that `console.log(length);` is called. And since `length` is a `const` (constant) that cannot be reassigned, it would be 3. 
11. The code prints nothing, but returns `[ 50, 100, 150 ]`. None of the lines calls the funtion `console.log()`. discounted[0] = (100 * 0.5), discounted[1] = (200 * 0.5), and discounted[2] = (300 * 0.5).
12. 
- A. student.name
- B. student['Grad Year']
- C. student.greeting()
- D. student['Favorite Teacher'].name
- E. student.courseLoad[0]
13. 
- A. '32'
  
  Because integer 2 is recognized as the string '2', and the output is simply displaying the combination of two strings, which is '32'.
- B. 1
  
  Because the operator `-` is used for subtraction, and string '3' is automatically converted to number 3, and the output is 3 - 2 = 1.
- C. 3
  
  Because 3 is an integer, the `+` operator is used for addition, and `null` is equivalent to 0, so the answer is 3 + 0 = 3.

- D. '3null'
  
  Because '3' is a string, the `+` operator is used for concatenation, and `null` is recognized as a string `'null'`, so the answer is the combination, which is '3null'. 

- E. 4
  
  Because true maps to 1, 3 + 1 = 4.

- F. 0
  
  Because false maps to 0, and null is equivalent to 0, so it is 0 + 0 = 0.

- G. '3undefined'
  
  Because '3' is a string, and undefined is also recognized as a string. The asnwer is simply '3undefined'.

- H. NaN
  
  The string '3' is converted to the number 3 because the minus operator is used. However, since undefined is not a number, the expression cannot be evaluated as a numerical subtraction. Therefore, the result is NaN.

14. 
- A. true
  
  Because when comparing values of different types, JavaScript converts the values to numbers. Therefore '2' is converted to 2, and 2 > 1 is true.

- B. false
  
  When comparing values of different types, JavaScript converts the values to numbers. '2' is converted to 2, '12' is cnverted to 12, and 2 < 12 is false.

- C. true
  
  When comparing values of different types, JavaScript converts the values to numbers. '2' is converted to 2, and 2 == 2 is true.

- D. false
  
  A strict equality operator `===` checks the equality without type conversion. Since integer 2 and string '2' are different types, it returns false. 

- E. false
  
  When comparing values of different types, JavaScript converts the values to numbers. `true` is converted to 1, and 1 == 2 is false.

- F. true
  
  The Boolean() function in JavaScript returns true for any non-zero number, and 2 is a non-zero number. So the expression Boolean(2) returns true. Therefore, true === true returns true (same value, same type). 

15.  The `==` operator would try to convert the values being compared to a unified type before comparing. However the `===` operator does not perform any type coercion. 
16.  See [part2-question16.js](part2-question16.js).
17.  The result is [ 2, 4, 6 ]. The function `modifyArray` is called with array `[1,2,3]` and a callback function `doSomething`. The function initializes an empty array. Using a `for` loop, the function iterates through the input array and calls the `doSomething` function for each iteration. `doSomething` doubles the number. The result of calling callback with the current element is added to the `newArr` array. After all elements have been processed, the `newArr` is returned with the doubled values.
18.  See[part2-question18.js](part2-question18.js)
19.  
```
1
4
3
2
```
