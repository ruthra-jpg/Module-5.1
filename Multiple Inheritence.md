# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```
# Class 1: For Addition
class Calculation1:
    def Summation(self, a, b):
        return a + b

# Class 2: For Subtraction
class Calculation2:
    def Subtraction(self, a, b):
        return a - b

# Derived Class: Inheriting from both Calculation1 and Calculation2
class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        if b == 0:
            return "Division by zero is not allowed"
        return a / b

# --- Main Program ---
# Step 1: Get user input
a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

# Step 2: Create object of Derived class
obj = Derived()

# Step 3: Perform operations
sum_result = obj.Summation(a, b)
sub_result = obj.Subtraction(a, b)
div_result = obj.Division(a, b)

# Step 4: Display results
print("\n--- Arithmetic Operations Result ---")
print(f"Addition of {a} and {b} = {sum_result}")
print(f"Subtraction of {a} and {b} = {sub_result}")
print(f"Division of {a} and {b} = {div_result}")
Enter first number: 20
Enter second number: 5
```
## Output Example
--- Arithmetic Operations Result ---
Addition of 20.0 and 5.0 = 25.0
Subtraction of 20.0 and 5.0 = 15.0
Division of 20.0 and 5.0 = 4.0
