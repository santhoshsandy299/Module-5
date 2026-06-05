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
class NAME:
    def __init__(self,name):
        self.name=name
class Age(NAME):
    def __init__(self,name,age):
        super().__init__(name)
        self.age=age
class Id(Age):
    def __init__(self,name,age,id):
        super().__init__(name,age)
        self.id=id
    def diplay(self):
        print(self.name,self.age,self.id)
name=input()
age=int(input())
id=int(input())
c=Id(name,age,id)
c.diplay()
```

## Sample Output
<img width="914" height="216" alt="508684130-8dc15778-f063-4118-891a-11970156275d" src="https://github.com/user-attachments/assets/6aff1da4-92e4-480e-ad10-bad81c1a8fac" />

## Result:
Thus the program that uses multilevel inheritance to get and display a person’s name, age, and id executed successfully.
