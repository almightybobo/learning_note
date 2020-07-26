# Udacity - C++ For Programmars Lesson 10: Templates

## Why Template
- can write a function once and use it over and over for different variable types

## Example
```  
  template <typename T>  //tell the compiler we are using a template
  // T represents the variable type. Since we want it to be for any type, we use T
  T  functionName (T parameter1,T parameter2, ...); 
  T functionName (T  parameter1,T  parameter2,...)
  {
      function statements;
  }
```

## Also can use on class
```
template <class T>
```
- The member functions must all be treated as generic functions. You will have to add the template command to each member function.


## Ref
- http://www.cplusplus.com/doc/oldtutorial/templates/
