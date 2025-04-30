### Question 1: What will happen at line 12 and why? If the code causes an error, explain why. 
The code causes an error, since i is a loop variable and the print statement is outside the scope of the for loop.

### Question 2: What will happen at line 13 and why?
Line 13 will print the last value that `discountedPrice` was assigned inside the `for` loop. Since `var` is function-scoped, `discountedPrice` is still accessible outside the loop. In this case, it will print the discounted price for the last element in the array: `150`.

So, the output will be: 150

### Question 3: What will happen at line 14 and why?
Line 14 will print the value of `finalPrice` after the loop finishes executing. Since `var` is function-scoped and the variable was declared outside the loop, it retains the last value assigned inside the loop.

In this case, `finalPrice` will be: 150

### Question 4: What will this function return? Give a brief explanation why.

The function will return: [50,100,150]
This happens because each price in the array is multiplied by `(1 - discount)`, which is `0.5`. The resulting values are rounded and pushed into the `discounted` array. There are no errors, and the logic works correctly with `var`.

### Question 5: What will happen at line 12 and why?

The code throws a `ReferenceError` at line 12 because the variable `i` was declared using `let` inside the `for` loop, which gives it **block scope**. This means `i` is not accessible outside of the loop block. Therefore, trying to log `i` outside the loop results in an error.

### Question 6: What will happen at line 13 and why?

The code will throw a `ReferenceError` at line 13 because `discountedPrice` was declared using `let` inside the `for` loop, which means it is **block-scoped**. It cannot be accessed outside of the `for` block, and therefore trying to log it causes an error.

### Question 7: What will happen at line 14 and why?

Line 14 will successfully print `150`. The variable `finalPrice` was declared using `let` outside the loop, so it is accessible throughout the function. During the loop, it was repeatedly reassigned, and after the final iteration (300 at 50% discount), its value became `150`. There is no error.

### Question 8: What will this function return? Give a brief explanation.

The function will return:[50,100,150]. Each price is multiplied by `(1 - discount)` which is `0.5`, resulting in a 50% discount. The result is rounded to two decimal places and added to the `discounted` array. No errors occur because all variables are correctly declared with `let` and used within their scope.

### Question 9: What will happen at line 11 and why?

Line 11 will throw a `ReferenceError` because the variable `i` is declared with `let` inside the `for` loop, which makes it **block-scoped**. This means `i` is not accessible outside the loop, and attempting to log it causes an error.

### Question .0: What will happen at line 12 and why?

Line 12 will print `3` to the console. The variable `length` is declared using `const` in the function scope and assigned the value `prices.length`. Since it is accessible throughout the function and not reassigned, no error occurs and the value is printed successfully.

### Question .1: What will this function return? Give a brief explanation.

The function returns: [50,100,150], because each price is multiplied by `(1 - discount)` to apply a 50% discount. The result is stored in `discountedPrice`, and pushed into the `discounted` array. All variables use `let` or `const` and are scoped correctly, so the function runs without any errors.

### Question .2: JavaScript Object Property Access

A- student.name
B- student["Grad Year"]
C- student.greeting()
D- student["Favorite Teacher"].name
E- student.courseLoad[0]

### JavaScript Type Conversion & Basic Operators

### Question .3: Arithmetic

A:
Output: '32'
Explanation: The `+` operator with a string causes string concatenation. 2 is converted to '2'.
B:
Output: 1
Explanation: The `-` operator triggers numeric coercion. '3' becomes 3, then 3 - 2 = 1.
C:
Output: 3
Explanation: `null` is coerced to 0 in arithmetic, so 3 + 0 = 3.
D:
Output: '3null'
Explanation: `null` is coerced to the string 'null', so this is string concatenation.
E:
Output: 4
Explanation: `true` becomes 1 in numeric context. 1 + 3 = 4.
F:
Output: 0
Explanation: `false` → 0, `null` → 0, so 0 + 0 = 0.
G:
Output: '3undefined'
Explanation: `undefined` is converted to the string 'undefined'. So this is string concatenation.
H:
Output: NaN
Explanation: `'3'` is coerced to number 3, but `undefined` is coerced to NaN. 3 - NaN = NaN.

### Question .4: Comparison
A:  Output: true
    Explanation: '2' is coerced to number 2, so 2 > 1 = true.
B:  Output: false
    Explanation: Both operands are strings, so comparison is lexicographic. '2' > '1', so '2' < '12' is false.
C:   Output: true
    Explanation: `==` allows type coercion. '2' is coerced to number 2, and 2 == 2.
D:   Output: false
    Explanation: `===` checks both value and type. Number 2 !== String '2'.
E:  Output: false
 Explanation: `true` becomes 1, so 1 == 2 is false.
F: Output: true
  Explanation: `Boolean(2)` is `true`, and both sides are Boolean `true`, so types and values match.

### Question .5: Explain difference between == and === operators
	•	== is the loose equality operator. It compares values after performing type coercion, if necessary.
	•	=== is the strict equality operator. It compares both value and type, and no type coercion is done.



