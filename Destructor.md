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
## Program
```
class demo:
    def __init__(self):
        self.status="Alive"
    def __del__(self):
        print("The object no longer exists")
a=demo()
print(a.status)
```
## 🧪 Output
<img width="964" height="219" alt="508683843-a7b0a93d-60ef-4303-a100-e45895dc50bb" src="https://github.com/user-attachments/assets/9aecc176-6737-48a7-bbcc-5ded06a5d529" />


## Result
Thus the program demonstrates how to implement a destructor in Python using a simple class has been executed successfully
