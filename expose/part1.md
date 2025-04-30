### Question 1: What is printed by line 9?
`values added: 20` is printed. The variable declared with `var` inside the `if` block is accessible throughout the function due to function-level scoping.

---

### Question 2: What is printed by line 13?
`final result: 20` is printed. Since `var` does not have block scope, the variable `result` declared inside the `if` block is still accessible outside of it within the function.

---

### Question 3: Why should you not use `var`?
You should avoid using `var` because:

- It does **not respect block-level scope**, which can lead to confusing bugs and unintended behavior.
- Variables declared with `var` are **hoisted**, meaning they are accessible before they are actually declared, which can be error-prone.
- It allows **re-declaration** of variables within the same scope, making your code harder to maintain and debug.

### Question 4: What is printed by line 9?
`values added: 20` is printed. Since `add` is `true`, the code inside the `if` block runs. The variable `result` is declared with `let`, assigned the value `10 + 10`, and logged inside the block.

### Question 5: What is printed by line 13?
The code throws a **ReferenceError** because `result` is declared with `let` inside the `if` block, making it block-scoped. It is not accessible outside the `if` block, so `console.log('final result: ', result);` causes an error.

### Question 6: What is printed by line 9?
The code throws a **TypeError** at line 7 (`result = num1 + num2`) before it reaches line 9. You cannot reassign a variable declared with `const`. Therefore, **nothing is printed** on line 9.

---

### Question 7: What is printed by line 13?
Line 13 is **never reached** because the program crashes before that due to the reassignment of a `const` variable. So, nothing is printed, and a **TypeError** is raised earlier in execution.

---