## Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```
class student:
    def __init__(self):
        print("This is non parametrized constructor")
    def name(self,a):
        print("Hello",a)
a=input()
obj=student()
obj.name(a)
```

## Output

<img width="1045" height="274" alt="image" src="https://github.com/user-attachments/assets/e5538bdb-9b8a-4312-a56e-03b4caec5097" />

## Result
Thus, the program demonstrates how to implement a non-parameterized constructor in Python using a simple class and has been executed successfully

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
<img width="964" height="219" alt="image" src="https://github.com/user-attachments/assets/a7b0a93d-60ef-4303-a100-e45895dc50bb" />


## Result
Thus the program demonstrates how to implement a destructor in Python using a simple class has been executed successfully

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
```
class Details:
    def __init__(self,id,name,gen):
        self.id=id
        self.name=name
        self.gen=gen
class Doctor(Details):
    def __init__(self,id,name,gen,hos,dept):
        super().__init__(id,name,gen)
        self.hos=hos
        self.dept=dept
    def display(self):
        print("Doctor Object")
        print("Id: ",self.id)
        print("Name: ",self.name)
        print("Gender: ",self.gen)
        print("Hospital: ",self.hos)
        print("Department: ",self.dept)
class Patient(Details):
    def __init__(self,id,name,gen,hos,dept):
        super().__init__(id,name,gen)
        self.hos=hos
        self.dept=dept
    def display(self):
        print("\nPatient Object")
        print("Id: ",self.id)
        print("Name: ",self.name)
        print("Gender: ",self.gen)
        print("Hospital: ",self.hos)
        print("Department: ",self.dept)
id=int(input())
name=input()
gen=input()
hos=input()
dept=input()

pid=int(input())
pname=input()
pgen=input()
phos=input()
pdept=input()

a=Doctor(id,name,gen,hos,dept)
b=Patient(pid,pname,pgen,phos,pdept)
a.display()
b.display()
```
## Sample Output
<img width="941" height="500" alt="image" src="https://github.com/user-attachments/assets/b0c4c08d-736a-4268-acfb-52c2cc4e026b" />

## Result:
Thus the program that uses Hierarchical Inheritance to input and display Doctor and Patient details hase been executed successfully.

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
<img width="914" height="216" alt="image" src="https://github.com/user-attachments/assets/8dc15778-f063-4118-891a-11970156275d" />

## Result:
Thus the program that uses multilevel inheritance to get and display a person’s name, age, and id executed successfully.

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
class Calculation1:  
    def Summation(self,a,b):  
        return a+b;  
class Calculation2:  
    def sub(self,a,b):  
        return a-b;  
class Derived(Calculation1,Calculation2):  
    def Divide(self,a,b):  
        return a/b;  
a=int(input())
b=int(input())
d = Derived()  
print(d.Summation(a,b))  
print(d.sub(a,b))  
print(d.Divide(a,b))  
```
## Output Example
<img width="997" height="218" alt="image" src="https://github.com/user-attachments/assets/53f83599-5aae-4f0f-bf08-887be99d52cc" />

## Result:
Thus the program demonstrates multiple inheritance by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes has been executed successfully.
