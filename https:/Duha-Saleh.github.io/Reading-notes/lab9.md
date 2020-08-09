FUNCTIONAL
PROGRAMMING
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

What is a pure function?
It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects.
Reading Files
If our function reads external files, it’s not a pure function — the file’s contents can change.

Random number generation
Any function that relies on a random number generator cannot be pure.

Pure functions benefits
The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D
Immutability
Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

how do we handle mutability in iteration? Recursion!
Referential transparency
Basically, if a function consistently yields the same result for the same input, it is referentially transparent. pure functions + immutable data = referential transparency With this concept, a cool thing we can do is to memoize the function.

Functions as first-class entities can:
refer to it from constants and variables pass it as a parameter to other functions return it as result from other functions The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

Higher-order functions
When we talk about higher-order functions, we mean a function that either: takes one or more functions as arguments, or returns a function as its result.

Examples :

Filter : Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection.
Map The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.
Reduce The idea of reduce is to receive a function and a collection, and return a value created by combining the items.
A hash function is used to map a given key

