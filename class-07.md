SIMPLE OR PRIMITIVE DATA TYPES
JavaScript has five simple (or primitive) data types:
1. String
2. Number
3. Boolean
4. Undefined (a variable that has been declared, but
no value has been assigned to it yet)
5. Null (a variable with no value - it may have had
one at some point, but no longer has a value)
As you have seen, both the web browser and the
current document can be modeled using objects
(and objects can have methods and properties).
But it can be confusing to discover that a simple
value (like a string, a number, or a Boolean) can have
methods and properties. Under the hood, JavaScript
treats every variable as an object in its own right.
St ring: If a variable, or the property of an object,
contains a string, you can use the properties and
methods of the String object on it.
Number: If a variable, or property of an object,
stores a number, you can use the properties and
methods of the Number object on it (see next page).
Boolean: There is a Boo 1 ean object. It is rarely used.
(Undefined and null values do not have objects.)
COMPLEX DATA TYPE
JavaScript also defines a complex data type:
6.0bject
Under the hood, arrays and functions are considered
types of objects.
ARRAYS ARE OBJECTS
As you saw on p118, an array is a set of key/value
pairs (just like any other object). But you do not
specify the name in the key/value pair of an array - it
is an index number.
like other objects, arrays have properties and
methods. On p72 you saw that arrays have a
property called 1 ength, which tells you how many
items are in that array. There is also a set of methods
you can use with any array to add items to it, remove
items from it, or reorder its contents. You will meet
those methods in Chapter 12.
FUNCTIONS ARE OBJECTS
Technically, functions are also objects. But they
have an additional feature: they are callable, which
means you can tell the interpreter when you want to
execute the statements that it contains. 
