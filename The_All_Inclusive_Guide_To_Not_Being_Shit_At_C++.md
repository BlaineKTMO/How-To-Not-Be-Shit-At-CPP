# You're shit at C++
That's not a bad thing, C++ is an incredibly complicated language. Here's some things you need to learn before you walk around touting you know C++.

If you don't want to mess around with an IDE, use this for the excercises: https://www.jdoodle.com/online-compiler-c++

## Introduction
Here's a *not bad* series on some basic C++ / Programming fundamentals: [youtube](https://www.youtube.com/watch?v=ea6YHMHcS0o&list=PL7Sp69foM4tsgkgZ71LW-SuAAtzjQr5XX&index=4)

This covers topics like:
- OOP
    - Encapsulation
    - Polymorphism
    - Inheritance
    - (It doesn't cover abstraction)
- Structs v. classes (Read: C-style v. C++ style)
- RAII (How not to blow your leg off)
- Constructors/destructors
    - Initialization lists
    - Defaults
    - More stuff on not blowing away appendages
- Const
- Operator Overloading

This is a good *starting point* but it neither has the breadth or depth.

## What is a value?
- Rvalue vs Lvalue
- std::move
- Move constructors and assignment operators

## Structs v. Objects
- What is a struct? [youtube](https://www.youtube.com/watch?v=IW16boBvQpc)
    - Exercise:
    ```
    Create a Robot struct that defines a drive type, number of wheels, and a name. Try using enumeration to define the drive type :)
    ```
- Important Questions:
    - What is the *pretty much only* difference between a struct and an object in C++?
        - Hint: Think OOP. Can we add methods? Can we define attributes as public/private?
    - What are some scenarios you would actually use a struct for? (Best practice)

## Memory management
- Pointers and References (Making sure your program doesn't use 2GB of memory)
    - What is a pointer? [Youtube](https://www.youtube.com/watch?v=2ybLD6_2gKM)
    - Write a not so simple program:
    ```
    To show you're not shit at pointers, write a simple C++ program that iterates over a string and prints all possible permutations. Hint: Use recursion.

    Ex. "ABC" should print "ABC ACB BAC BCA CBA CAB"
    ```
    - Applications of pointers
        - [Two Pointer Approach for LeetCodes](https://www.youtube.com/watch?v=On03HWe2tZM)
        - [Pointer Arithmetic](https://www.youtube.com/watch?v=q24-QTbKQS8)
- Double pointers [youtube](https://www.youtube.com/watch?v=k6ESk9zafHM)
    - Pay attention to the example portion where he writes his own pthread function.
    - Write a simple program:
    ```
    Create a person struct with attributes name and age. Use a double pointer to create an array of people. Pass this into a function along with an array of names to iteratively set the name of each person.
    ```
- Smart Pointers
    - std::unique_ptr
    - std::shared_ptr
    - std::weak_ptr
- Dynamic memory allocation (How not to leak!!)
    - Memory Leaks
    - Dangling Pointers

## Standard Template Library
Stop. It's already been written.
- Containers
    - std::vector
    - std::map
    - std::set
- Iterators (The modern way to loop over a sequential container)
    - Excercise:
        ```
        In the previous double pointer excercise, replace the double pointer with a std::vector and use iterators to loop over the vector.
        ```
- Algorithm
    - std::sort and more
    - std::accumulate
- Functional programming (not related but powered by the above)
    - Functors / lambdas

## Everything is a stream
- std::cin, std::cout, std::cerr
- file streams 
- string streams

## OOP (But make it C++!)
C++ brings along some smart implementations that extend OOP functionality.

- Pure Virtual
- Abstract / Interface
- Multiple Inheritance
- Friends (Get some)

## Generic Programming
- Templates
- Template Specialization
- Variadic Templates


## Error Handling
- Try/Catch/Except
- std::runtime_error, std::exception
- Deeper into RAII

## Multithreading
- std::thread, std::async
- Mutex/Semaphore (Oh no!)
    - std::lock_gaurd, std::mutex

## The deep stuff
- Lambdas
- Type trains
- constexpr (similar to macros)
- macros
- Literals

## Best practices
- RAII (it's important)
- Three/Five/Zero
- DRY
- const

## Modern C++
There was a transition at C++ 11 that makes it the starting point of "Modern C++"
- Extra features (auto, range-based for)
