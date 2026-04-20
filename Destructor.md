# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
🧾 Program

# Destructor in Python

class Demo:
    # Constructor
    def __init__(self):
        self.status = "Alive"
        print("Object is created. Status:", self.status)

    # Destructor
    def __del__(self):
        print("Destructor called. Object is being destroyed.")

# Creating object
obj = Demo()

# Deleting object
del obj

🧪 Output

<img width="320" height="90" alt="Destructor Output" src="https://github.com/user-attachments/assets/2d1b4a9c-0fa1-4e32-8f82-2fd15e5f7f29" />🏁 Result
## Result
The program successfully demonstrated the use of a destructor in Python to indicate when an object is destroyed.
