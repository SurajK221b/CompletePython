=====================================================================
                        PYTHON DATA TYPES - THEORY & INTERVIEW
=====================================================================

What are Data Types?
---------------------
A Data Type defines the kind of value a variable holds.

Python is dynamically typed, meaning the interpreter assigns types at runtime.
Use `type()` to check the type of a variable:
    x = 10
    print(type(x))  # <class 'int'>


=====================================================================
BUILT-IN DATA TYPES (CORE CATEGORIES)
=====================================================================

1. NUMERIC TYPES
-----------------
A. int       => Integer numbers
   Example: x = 10
   Operations: +, -, *, /, %, //, **, bit_length()

B. float     => Decimal numbers
   Example: pi = 3.14
   Supports scientific notation (e.g., 1.5e2)

C. complex   => Complex numbers
   Example: z = 2 + 3j
   Properties: z.real, z.imag


2. STRING (str)
-----------------
Immutable sequence of Unicode characters.
   name = "Suraj"

String Methods:
   s.lower(), s.upper(), s.strip(), s.find(), s.replace(), s.split()

String Operations:
   "abc" + "xyz"         => Concatenation
   "abc" * 3             => Repetition
   "a" in "apple"        => Membership
   len("hello")          => Length


3. LIST (list)
-----------------
Ordered, mutable collection.
   fruits = ["apple", "banana", "mango"]

Common Methods:
   append(), insert(), pop(), remove(), reverse(), sort(), index()

Common Operations:
   fruits[0]             => Indexing
   fruits[1:3]           => Slicing
   "apple" in fruits     => Membership


4. TUPLE (tuple)
-----------------
Ordered, immutable collection.
   coords = (10.5, 20.0)

Supports indexing, slicing.
Hashable => can be used as dictionary keys.


5. SET (set)
-----------------
Unordered collection of unique elements.
   colors = {"red", "blue", "green"}

Set Operations:
   add(), remove(), discard(), union(), intersection(), difference()


6. DICTIONARY (dict)
---------------------
Unordered key-value pairs.
   person = {"name": "Suraj", "age": 30}

Dictionary Methods:
   get(), keys(), values(), items(), update(), pop()


7. BOOLEAN (bool)
-------------------
True / False
   x = 5 > 3         => True
   bool("")          => False
   bool("hello")     => True


8. NONE TYPE (NoneType)
-------------------------
Represents absence of value.
   x = None


9. BINARY TYPES (Advanced Use)
-------------------------------
- bytes
- bytearray
- memoryview


=====================================================================
TYPE CONVERSION / TYPE CASTING
=====================================================================
int("100")         => 100
float("3.14")      => 3.14
str(100)           => "100"
list("abc")        => ['a', 'b', 'c']
set([1,2,2,3])     => {1, 2, 3}


=====================================================================
INTERVIEW QUESTIONS – PYTHON DATA TYPES
=====================================================================

THEORY-BASED QUESTIONS
-----------------------
1. What are the built-in data types in Python?
2. How is a tuple different from a list?
3. What is the difference between is vs ==?
4. What is NoneType used for?
5. What data types are mutable and immutable in Python?
   - Mutable: list, dict, set
   - Immutable: int, float, str, tuple, bool

CODE-BASED QUESTIONS
----------------------
1. Output of:
       x = [1, 2, 3]
       y = x
       y.append(4)
       print(x)
   => Output: [1, 2, 3, 4]

2. Difference between dict.get('x') and dict['x']?
   - get() returns None if key not found
   - dict['x'] throws KeyError

3. How to convert a list with duplicates to a unique set?
       list1 = [1,2,2,3]
       unique = set(list1)

4. Is this valid?
       a = (1, 2)
       b = (1, 2)
       print(a is b)
   => Output: False (Identity may differ)

5. How can we store multiple values in a single variable?
   - Use tuple, list, or dict depending on use case


=====================================================================
END OF MODULE
=====================================================================
