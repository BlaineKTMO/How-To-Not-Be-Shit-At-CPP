# You're shit at C++
That's not a bad thing, C++ is an incredibly complicated language. Here's some things you need to learn before you walk around touting you know C++.

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

## Memory management
- Pointers and References (Making sure your program doesn't use 2GB of memory)
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
- Algorithm
    - std::sort and more
    - std::accumulate
- Functional programming (not related but powered by the above)
    - Functors / lambdas

## What is a value?
- Rvalue vs Lvalue
- std::move
- Move constructors and assignment operators

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
