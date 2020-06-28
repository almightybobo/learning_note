# Udacity - C++ For Programmars Lesson 2: Compliation and Execution

## Compliling
- the process of translating the code that you've written into machine code that processors understand
- scripting languages (ex. Python, JavaScript) don't need to compile
  - the interpreter (or a similar system) is responsible for compiling code on the fly in a process known as just-in-time compiling
  - To the user, compilation and execution of scripting languages are effectively a single action.
- compiled languages -> compiled to an executable, non-human readable file with machine code that the processor can run
- compiled tools
  - g++
  - CMake(high-level build tool, does not compile code) with make(low-level build tool to manage compiling from source)

## Object Files
- compiling source code results in an object file
- contains machine code but may not be executable in and of itself
- depended upon object files might come from other source files within the same project or from external or system libraries
- in order to be executable, object files need to be linked together

## Linking
- the process of creating an executable by effectively combining object files
- the linker resolves symbolic references between object files and outputs a self-contained binary with all the machine code needed to execute
- dynamic linking: symbolic references resolved at runtime 
  - pros: not linked within binaries, which keeps the overall file size down
  - cons: if the library changes at any point, your code will automatically link to the new version. Like any changing dependency, difficult to fix and surprising bugs sometimes arise when versions change. 

## Compiling to Executable with a Compiler
- challenges with using gcc alone (because most C++ projects are large)
  - need to pass the paths for all of the project's source header files and cpp files to gcc
  - GCC in and of itself is not smart enough to recognize what files in your project have changed and which haven't, and as such will recompile binaries needlessly - you'd need to manually change your gcc calls for the same optimizations
- has tools to solve the problems


