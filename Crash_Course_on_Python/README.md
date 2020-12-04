# Week-1: Hello Python!
## What is Python?
Python is a general purpose scripting language.

Benefits of using Python includes programming in Python usually feels similar to using a human language.

In programming, an interpreter is the program that reads and executes code. The Python interpreter is the program that reads what is in the recipe and translates it into instructions for your computer to follow.

# Week-2: Basic Python Syntax

## Expression and Variables
### Data Types
There are different data tpyes in Python. Some of the examples include:
* String which represents text wrapped in quotation marks to be manipulated by a script
* Integer which represents whole numbers without a fraction (ex. 1)
* Float which represents real numbers like a number with a fractional part (ex. 2.5)

Generally, computer doesn't know how to mix different data types - it results "TypeError".

If you're ever not 100 percent sure what data types a certain value is, Python gives you a handy way to find out. You can use the type function, to have the computer tell you the type

### Variables
* **Variables** are names that we give to certain values in our programs - variables are like containers for data.
    * Values can be of any data type; numbers, strings or even the results of operations.
    * Variables are important in programming because they let you perform operations on data that may change
* **Assignment** is the process of storing a value inside a variable.
    * A value is assigned to a variable by using the equal sign in the form of variable equals value
* An **expression** is a combination of numbers, symbols or other variables that produce a result when evaluated.

Below are some restrictions when naming variables in Python
1. Key words or functions that Python reserves for its own cannot be used as variable names
2. Variable names can't have any spaces and they must start with either a letter or an underscore
3. Variable names can only be made up of letters, numbers and underscores
4. Python variables are case sensitive

### Expressions, Numbers, and Type Conversion
* **Implicit conversion** takes plance when the interpreter automatically converts one data type into another.
* **Explicit conversion** takes place when a function is called to convert one data type into antother

---

## Functions
### Defining Functions
To define a function in Python,
1. Use the **def** keyword to define a function. The name of the function is what comes after the keyword. 
2. The parameters of the function are written between parentheses after the name.
3. The body of the function must be to the right of the definition.
Example:
    ```Python
    def greeting(name):
        print("Hello, " + name)
    ```

### Reutrning Values
The return statement allows us to:
* Combine calls to functions
* Perform more complex operations
* Makes the code more reusable
* **In Python, it can return more than one value**
 
* **Double slash operator (//)** is called **floor division**. A floor division divides a number and takes the integer part of the division as the result.
* **None** is a very special data type in Python used to indicate that things are empty or that they return nothing.

### Code Style
A few principles in mind to create good well styled code are:
1. Code to be self-documenting as possible
    * Self-documenting code is written in a way that's readable and doesn't conceal its intent. 
2. Leave a comment to add a bit of explanatory texts to the code
    * In Python, comments are indicated by the hash character

---

## Conditionals
### Compare Things
Equality operators allows us to take the result of the expressions and use them to make decisions
* a == b: a is equal to b
* a != b: a is different than b
* a < b: a is smaller than b
* a <= b: a is smaller or equal to b
* a > b: a is bigger than b
* a >= b: a is bigger or equal to b

Logical operators allow connecting multiple statements together and perform more complex comparisons
* a and b: True if both a and b are True. False otherwise.
* a or b: True if either a or b or both are True. False if both are False.
* not a: True if a is False, False if a is True.

**In Python uppercase letters are alphabetically sorted before lowercase letters**

### Branching with if Statements
**Branching** is the ability of a program to alter its execution sequence.

if block vs. defined function
| Similarities | Differences |
|:-|:-|
| * The keyword, either def or if, indicates the start of a special block
* Colon is used at the end of the first line
* The body of the function or the if block is indented to the right | * The body of the if block will only execute when the condition evaluates to true; otherwise, it skipped |

### else Statements
* The **modulo operator** is represented by the percentage sign (%) and __returns the remainder of the integer division between two numbers__. 
* **The integer division is an operation between integers that yields two results which are both integers, the quotient and the remainder.*
* When a return statement is executed, the function exits so that the code that follows doesn't get executed.

### elif Statements
The main difference between elif and if statements is that an elif block can be only written as as a companion to an if block.

---

# Week-3: Loops

## While Loops
### What is a while loop?
While Loops instruct computer to continuously execute the code based on the value of a condition. The difference between if statements and while loop is that the body of the block can be executed multiple times instead of just once.

**Initialization** is to give an initial value to a variable.

### Why initializing variables matters
When we forget to initialize the variable two different things can happen:
1. A name error when we forget to initialize a variable 
2. When we forget to initialize variables with the right value

### Infinite loops and how to break them
While loops:
* Use the condition to check when to exit
* The body of the while loop needs to make sure that the condition being checked will change

An **infinite loop**, a loop that keeps executing and never stops.

**Break** keyword can stop infinite loops but also to stop a loop early if the code has already achieved what's needed.

---

## for Loops
### What is for loop?
For loops iterate over a sequence of values. The for loop can iterate over a sequence of values of any type, not just a range of numbers.

The range function, range():
1. A range of numbers will start with the value 0 by default.
2. The list of numbers generated will be one less than the given value
3. The range function takes two parameters to the function instead of one to specify the first element of the list to generate
4. The range function takes a third parameter to change the size of each step (increments)

### Nested for Loops
**Nested for loops** are two for loops, one inside the other.

However, use caution when using nested for loops since the longer the list your code needs to iterate through, the longer it takes computer to complete the task. 

### Common Errors
The interpreter will refuse to iterate over a single element. This can be mitigated by:
1. Using range()
2. Make the loop iterate over a list with the single element

Since strings are iterable, above solution may be needed. 

for loops are best when you want to iterate over a known sequence of elements but when you want to operate while a certain condition is true, while loops are the best choice.

---

## Recursion
### What is recursion?
**Recursion** is the repeated application of the same procedure to a smaller problem. It tackles complex problems by reducing the problem to a simpler one by a function call itself until it reaches the **base case**.

In Python, a recursive function can be called up to 1,000 times.

---


# Week-4: Strings, Lusts and Dictionaries

## Learning Objectives
* Understand the difference between strings, lists, and dictionaries
* Manipulate strings in your code
* Create and use lists
* Create and use dictionaries

---

## String
### What is a string?
A **string** is a data type in Python that's used to represent a piece of text.

Strings can be concatenated to build longer strings by using the plus sign or multiplied by a number, which multiplies the content of the string that many times.

### The Parts of a String
The **string indexing** operation accesses the character in a given position or index using square brackets and the number of the position specified
* string[0]
* To access the last character of a string, use negative indexes
* A **slice** is the portion of a string that can contain more than one character (ex. string[1:4])

### Creating New Strings
Strings in Python are immutable, meaning __they can't be modified__.

### Formatting Strings
String operations
* len(string) Returns the length of the string
* for character in string Iterates over each character in the string
* if substring in string Checks whether the substring is part of the string
* string[i] Accesses the character at index i of the string, starting at zero
* string[i:j] Accesses the substring starting at index i, ending at index j-1. If i is omitted, it's 0 by default. If j is omitted, it's len(string) by default.

String methods
* string.lower() / string.upper() Returns a copy of the string with all lower / upper case characters
* string.lstrip() / string.rstrip() / string.strip() Returns a copy of the string without left / right / left or right whitespace
* string.count(substring) Returns the number of times substring is present in the string
* string.isnumeric() Returns True if there are only numeric characters in the string. If not, returns False.
* string.isalpha() Returns True if there are only alphabetic characters in the string. If not, returns False.
* string.split() / string.split(delimiter) Returns a list of substrings that were separated by whitespace / delimiter
* string.replace(old, new) Returns a new string where all occurrences of old have been replaced by new.
* delimiter.join(list of strings) Returns a new string with all the strings joined by the delimiter

---

## Lists
### What is a list?
Square brackets are used to indicate where the list starts and ends in Python.

In Python, strings and lists are both examples of **sequences**. There are other sequences too, and they all share operations like:
* Iterating over them using for-loops
* Indexing using the len function to know the length of the sequence
* Using plus to concatenate two sequences
* Using in to verify if the sequence contains an element

### Modifying the Contents of a List
One of the ways that lists and strings are different is that lists are mutable. Which is another fancy word to say that they can change. This means we can add, remove, or modify elements in a list.
* The append method adds a new element at the end of the list. 
* The insert method inserts an element in a different position, instead of at the end, by taking an index as the first parameter and an element as the second parameter.
* The remove method removes an element 
* The pop method can also remove an element and receives an index

### Lists and Tuples
* **Strings** are sequences of characters and are **immutable**.
* **Lists** are sequences of elements of any type and are **mutable**.
* **Tuples** are sequences of elements of any type that are **immutable**.
    * When using tuples the position of the elements inside the tuple have meaning.
    * Tuples can be **unpacked** whichwe can turn a tuple of elements into separate variables. 

Examples of tuples include:
* When a function returns more than one value, it's returning a tuple.
* Store a filename and it's size
* Store the name and email address of a person
* Store a date and time and the general health of the system at any point in time

### Iterating over Lists and Tuples
Use **enumerate** method when iterate over lists or tuples.

Using range method works BUT it's more idiomatic in Python to iterate through the elements of the list directly or using enumerate when we need the indexes.

### List Comprehension
Since creating lists based on sequences is such a common task, Python provides a technique called **list comprehension**, which allows it to be done in just one line. __List comprehensions let us create new lists based on sequences or ranges.__

---

## Dictionaries
### What is a dictionary?
**Dictionaries** take the form of pairs of keys and values to store data.
* Dictionaries are mutable
* Unlike lists, elements cannot be accessed using their position

#### Definition
x = {key1:value1, key2:value2}

#### Operations
* len(dictionary) - Returns the number of items in the dictionary
* for key in dictionary - Iterates over each key in the dictionary
* for key, value in dictionary.items() - Iterates over each key,value pair in the dictionary
* if key in dictionary - Checks whether the key is in the dictionary
* dictionary[key] - Accesses the item with key key of the dictionary
* dictionary[key] = value - Sets the value associated with key
* del dictionary[key] - Removes the item with key key from the dictionary

#### Methods
* dict.get(key, default) - Returns the element corresponding to key, or default if it's not present
* dict.keys() - Returns a sequence containing the keys in the dictionary
* dict.values() - Returns a sequence containing the values in the dictionary
* dict.update(other_dictionary) - Updates the dictionary with the items coming from the other dictionary. Existing entries will be replaced; new entries will be added.
* dict.clear() - Removes all the items of the dictionary
---


## Credit
* [Coursera - Google IT Automation with Python](https://www.coursera.org/professional-certificates/google-it-automation?)
* [Kyungrae Kim](https://github.com/jeremymaya/google-it-automation-with-python)
