Prateek Sinha

24070123077

ENTC A3

# C++ Programs – Function Calling Techniques and Salary Increment Project

This repository contains four C++ programs demonstrating different methods of function calling and a practical application project that evaluates salary increments based on performance criteria.

This document explains two fundamental function calling methods in C++:

- **Call by Value**
- **Call by Reference**

Understanding these techniques is essential for managing how data is passed and manipulated between functions in C++ programs.

---

## Call by Value

### Theory

**Call by Value** is a function calling method where the actual values of variables are **copied** into the function parameters. The function works with these **copies**, meaning any changes made to the parameters inside the function **do not affect** the original variables.

This approach ensures data **safety**, as the original variables remain unchanged. However, it can be less efficient for large data types because it involves copying the data.

### Advantages

- Protects original data from unintended changes.
- Simple and easy to understand.
- Useful for read-only operations or when data integrity is important.

### Limitations

- Cannot modify the caller's variables.
- Inefficient for large objects due to copying overhead.

### Use Cases

- Mathematical operations where inputs shouldn't be altered.
- Functions that don't need to modify external variables.
- Safe API design where defensive copying is required.

---

## Call by Reference

### Theory

**Call by Reference** passes the **actual variables** (not copies) to the function. This is done using **references**, which are essentially **aliases** for the original variables. Any modification made to the parameters inside the function **directly affects** the original variables.

It provides a clean and safe way to allow functions to modify the caller’s data, without the complexity of pointers.

### Advantages

- Allows direct modification of the caller’s variables.
- No need for address (`&`) or dereferencing (`*`) operators.
- More readable and safer than pointers.
- No extra memory usage from copying.

### Limitations

- Risk of unintended side effects if not handled carefully.
- Cannot be used with constants or literals directly.

### Use Cases

- Swapping values.
- Functions that need to return multiple outputs.
- Performance-critical applications avoiding unnecessary copies.
- Operator overloading and object manipulations.


---

##  Topic 1: Pass by Pointer

### Theory

**Pass by pointer** allows direct access and modification of the memory location of variables by passing their addresses to a function. This method enables the function to change the actual values of the variables outside its local scope.

### Algorithm

1. Declare two integer variables and initialize them.
2. Define a function that accepts pointers to integers.
3. Inside the function, use a temporary variable to swap the values via dereferencing.
4. In `main()`, call the function using the addresses of the variables.
5. Print the values before and after swapping.

---

##  Topic 2: Call by Reference

### Theory

**Call by reference** passes the actual variables to the function using references (aliases), allowing direct modification of the original variables. It offers similar functionality to pass by pointer but with simpler syntax and better readability.

### Algorithm

1. Declare two integer variables and initialize them.
2. Define a function that takes integer references as parameters.
3. Inside the function, use a temporary variable to swap the values.
4. Call the function directly with the variables (no `&` needed in the call).
5. Display values before and after swapping.

---

##  Topic 3: Call by Value

### Theory

**Call by value** sends copies of the actual arguments to the function. Any modifications within the function affect only the copies, leaving the original variables unchanged.

### Algorithm

1. Declare and initialize two integer variables.
2. Define a function that takes two integer parameters.
3. Swap the values using a temporary variable inside the function.
4. Call the function with original variables.
5. Print the values after the function call to show they remain unchanged.


---

##  Topic 4: Salary Increment Evaluation Project

### Theory

This program evaluates an employee’s eligibility for a 20% salary increment based on the following four performance criteria:

1. At least one research project completed.
2. At least one research publication made.
3. Profit of ₹100,000 or more generated.
4. At least one new project initiated by the firm.

If the employee satisfies **three or more** criteria, they receive a 20% salary increment.

### Algorithm

1. Initialize a counter to 0.
2. Prompt the user for:
   - Number of research projects
   - Number of research publications
   - Profit value
   - Number of new projects
3. Increment the counter for each criterion met.
4. Take the current salary as input.
5. If the counter ≥ 3:
   - Calculate and display a 20% incremented salary.
6. Else:
   - Display “no increment”.

### Conclusion

This project demonstrates a real-life use of decision-making structures and user input handling in C++. It effectively shows how conditional logic can drive business rule implementations like performance-based salary evaluation.

---

