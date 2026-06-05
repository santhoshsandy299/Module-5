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

<img width="941" height="500" alt="508684018-b0c4c08d-736a-4268-acfb-52c2cc4e026b" src="https://github.com/user-attachments/assets/fe5b64be-90b6-44b0-81e6-39a08f542fce" />
## Result:
Thus the program that uses Hierarchical Inheritance to input and display Doctor and Patient details hase been executed successfully.
