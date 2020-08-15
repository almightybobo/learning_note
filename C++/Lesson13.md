# Udacity - C++ For Programmars Lesson 13: Vectors and Iterators

## Object Oriented Class
- has many containers that are quite useful for programming
- ex.
```
// The vector has size 0 when we instantiate it.
std::vector<int> vectorInts; 
// We use 'resize' to change the size of the vector.
vectorInts.resize(6);
```
## Vector
- We use ::assign to add and define elements to the vector
- We instantiate an iterator for the vector class
```
std::vector<int>::iterator it;
```
- We use the iterator to cycle through the vector.
```
for (it = vectorInts.begin(); it != vectorInts.end(); ++it)
    std::cout<<*it<<" ";
```
- ref: http://www.cplusplus.com/reference/vector/vector/vector/
- vectorInts.assign(number of element, value) -> will write over the elements in the vector
- vectorInts.push_back(24) -> append in vector tail
- vectorInts.insert(it, -1) -> append in vector head
- vectorInts.clear() -> clear all elements in vector
- vectorInts.erase(vectorInts.begin()+4) -> clear an element in vector
- vectorInts.erase(vectorInts.begin()+1, vectorInts.begin()+3); -> clear a range of elements in vector
- vectorInts.pop_back() -> DOES NOT return a value! Only pop the last element in array

## Emplace vs. insert
- insert copies the values of the vector
- emplace does an in-place insertion
