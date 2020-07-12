# Udacity - C++ For Programmars Lesson 8: Classes

## Default
- make all members private: only other members of the class can access the data

## How to access the data in a class
- can use functions to access the data in a class
  - functions that access and/or modify data values in classes are called mutators

## Class Member
- use public in class and can create function, then outside can call function to get it

## Constructors
- executed whenever we create a new instance of the class
- used to set initial values of data members of the class
- do not return a value, including void

## Destructors
- called whenever an object goes out of scope
- just like a constructor, a destructor is called automatically
- cannot return value, cannot accept parameters
- must have the same name as the class (identified with a tilda (~) symbol)
- release memory that was allocated by the class constructor and member functions

## Helper Functions in Classes
- can perform tasks that are often requested or are easier to perform in the class itself

## Arrays and Classes
- can use a user defined object in an array
- Dog dogs[3] -> 3 Dog objects

