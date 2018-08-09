# Anatomy: A Python Program

Depending on the size and purpose of a given program, the structure can take a few different shapes. Approaches to program "shapes" are correlated to complexity and an increasing need for Best Practices, such as "clean," readable, and tested code.

Given a hypothetical project folder -- which we'll call `OurProject/` -- let's look at the anatomy of a **single-file program** in Python for a basic view.


e.g. **_employee.py_**
```python

# a. Define Employee class
class Employee:
    def __init__(self, name):
        self.name = name

    def __repr__(self):
        return f"< Employee: {self.name} >"

# b. Define Employees class -- as a _Manager_ -- handling incoming/outgoing Employee objects
class Employees(Employee):
    def __init__(self):
        self.cls = Employee
        self.all = []
 
    def __call__(self):
        return self.all

    def get(self, name: str):
        if name in self.all:
            index = self.all.index(name)
            return self.all[index]

    def __display__(self, names: list):
        for name in names:
            employee = self.get(name)
            print(employee)

    def hire(self, names: list):
        for name in names:
            hiree = self.cls(name)
            self.all.append(hiree)
        return self()

# 1. Define a set of data to work with or "do" something with
data = [
    "Ryan Ferguson",
    "Thom Yorke",
    "Kevin Mitnick",
    "Chuck Norris"
]

# 2. Initialize our Employees instance
Manager = Employees()

Company = Manager.hire(data)
print(Company)

# OUTPUT:
[< Employee: Ryan Ferguson >, < Employee: Thom Yorke >, < Employee: Kevin Mitnick >, < Employee: Chuck Norris >]
```
