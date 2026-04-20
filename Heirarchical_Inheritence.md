# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
 Program to demonstrate Multilevel Inheritance in Python

# Parent class
class Person:
    def __init__(self, name):
        self.name = name

    def getName(self):
        return self.name


# Child class (inherits Person)
class Age(Person):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

    def getAge(self):
        return self.age


# Grandchild class (inherits Age)
class Location(Age):
    def __init__(self, name, age, location):
        super().__init__(name, age)
        self.location = location

    def getLocation(self):
        return self.location


# Taking user input
name = input("Enter Name: ")
age = int(input("Enter Age: "))
location = input("Enter Location: ")

# Creating object of grandchild class
person1 = Location(name, age, location)

# Displaying details
print("\n--- Person Details ---")
print("Name:", person1.getName())
print("Age:", person1.getAge())
print("Location:", person1.getLocation())
Enter Name: Sarah
Enter Age: 28
Enter Location: Chennai

--- Person Details ---
Name: Sarah
Age: 28
Location: Chennai

