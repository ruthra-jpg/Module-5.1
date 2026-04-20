# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
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
## Sample Output
--- Arithmetic Operations Result ---
Addition of 20.0 and 5.0 = 25.0
Subtraction of 20.0 and 5.0 = 15.0
Division of 20.0 and 5.0 = 4.0
