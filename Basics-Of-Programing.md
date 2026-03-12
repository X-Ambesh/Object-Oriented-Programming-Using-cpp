
---

#### Procedure Oriented Programming (POP) 

A complete program is divided into small parts called functions. Each function performs a specific task. 

Follow the top down approach, where the main program is written first, and then the functions are defined later.

e.g. C, Fortran, Pascal, etc.

---

#### Object Oriented Programming (OOP)

OOP = Object Based + Inheritance

A language in whcih the program is divided into multile clases and objects. 

Bottom up approach, where the classes and objects are defined first, and then the main program is written later.

e.g. C++(Both POP & OOP  ), Java(OOP), Python(Both POP & OOP)

Features of OOP:

1. Polymorphism
2. Data Hiding
3. Inheritance
4. Abstraction
5. Encapsulation
6. Class and Object etc.
   
---

#### Object Based Programming (OBP)

A language in which the program is divided into multile clases and objects, but it does not support inheritance.

e.g. JavaScript, VBScript, etc.


#### 1  Polymorphism

To achieve more than one thing from single thing.

1. Operator Overloading
   
   - \+ to add and to concatenate in c++
   - \* to multiply and to repeat in c++

2. function overloading or method overloading

   - same name but different parameters
   - compile time polymorphism
  
#### 2 Data hiding 

- hiding data from outside world

#### 3 Abstraction

  - hiding complexity and showing only necessary details to the user
  - use the thing without knowing how it works
  - example:using mobile phone without knowing how it works
  - make a class for data hiding and for abstraction make class
   - Data hinding = Class &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Abstraction = Object
  
#### 4  Encapsulation
   Data hiding + Abstraction = Encapsulation

#### 5 Inheritance

A derived class(Child Class) can inherit from a base class(Superclass), which means it can use the properties and methods of the base class. 

1. Single Inheritance: A derived class inherits from a single base class.
2. Multiple Inheritance: A derived class inherits from more than one base class.
3. Multilevel Inheritance: A derived class inherits from a base class, which itself is derived from another base class.
4. Hierarchical Inheritance: Multiple derived classes inherit from a single base class.
5. Hybrid Inheritance: A combination of two or more types of inheritance.

#### Object

Everything having property and method is called object

- Property is a variable that belongs to an object

- Method is a function that belongs to an object

#### Class

Class is a blueprint for creating objects. It defines a set of properties and methods that the objects created from the class will have.

- Instance is an individual object created from a class. Each instance has its own set of properties and methods

#### There are two types of relationship between classes:

#### Is a relation or inheritance relationship
Is a relation is a relationship between two classes where one class is a subclass of another class. The subclass inherits the properties and methods of the superclass.

#### Has a relation 
Has a relation is a relationship between two classes where one class has a property that is an instance of another class. The class that has the property is called the "has a" class, and the class that is the property is called the "is a" class.

---

#### Errors in c++

There are three types of errors in c++:

1. Syntax errors or compilation errors: These are errors that occur when the code violates the syntax rules of the programming language. For example, forgetting to include a semicolon at the end of a statement or using an undeclared variable.
   

2. Logical errors or runtime errors: These are errors that occur when the code does not produce the expected output due to a mistake in the logic of the program. For example, using the wrong operator in a calculation or having an infinite loop.
   

3. Linker errors: These are errors that occur when the linker is unable to find the necessary libraries or object files to create an executable. For example, forgetting to include a library or having a mismatch between the function declarations and definitions.
   
   

