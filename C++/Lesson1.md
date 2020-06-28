# Udacity - C++ For Programmars Lesson 1: Basic

## include: < > v.s. " "
- angle brackets: Look in the directory where the standard libraries are kept
- double quotes: Look in the current directory, if the file is not there, then look in the directory where the standard libraries are stored

## using namespace std
- like global variable

## Basic console
- std::cout << "output info" << "\n";
- format output
  - use std::setw(n), n is an integer
  - use \t
- std::cin >> variable; (Warning: space will consider the end)
- include string, std::getline(std::cin, variableName); (space will not consider the end)
- convert the string variable to a numeric variable
  - include sstream
  - std::stringstream(stringVariable) >> numericVariable;


## Constant
- const int a = 100; -> cannot be changed during the program
- enum constant: programmer can create a new variable type and then assign a finite number of values to it
  - enum MONTH {Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec};
  - Jan=0, Feb=1 ...

## File IO
- include <fstream>
- ofstream, ifstream, fstream
- f.open(filename), f.close()

## Header File
- Header files contain information about how to do a task
- The main program contains information about what to do

## Reference
### C++ Style Guide
- Google style guide: https://google.github.io/styleguide/cppguide.html
- Modern C++ style guide: https://github.com/Microsoft/AirSim/blob/master/docs/coding_guidelines.md

### C++ Core Guide
- http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines



