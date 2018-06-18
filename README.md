# Functions and Scope

## SWABT
* Understand the use case for functions in programming (abstraction and reuse)
* Create and use functions in Python
* Demonstrate a clear understanding of variable scope by defining local and global variables
* Pass arguments to user-defined functions in order to re-use function code repeatedly 


### Functions 


A function is a block of organized, reusable code that is used to perform a single, related action. Functions provide better modularity for your application and a high degree of code reusing.

![](https://codesachin.files.wordpress.com/2016/04/220px-function_machine2-svg.png)

As you have already seen, Python gives you many built-in functions like print(), etc. but you can also create your own functions. These functions are called user-defined functions.


### Defining a Function

You can define functions to provide the required functionality. Here are simple rules to define a function in Python.

* Function blocks begin with the keyword `def` followed by the function name and parentheses ( ( ) ).

* Any input parameters or arguments should be placed within these parentheses. You can also define parameters inside these parentheses.

* The first statement of a function can be an optional statement - the documentation string of the function or docstring.

* The code block within every function starts with a colon (:) and is indented.

* The statement `return [some expression]` exits a function, optionally passing back an expression to the caller. A return statement with no arguments is written as `return None`.

### Syntax of a Function

A common syntax of a function in python may look like this:

```

def functionname( parameter1, parameter2 .. ):
   "function_docstring"
   function_processing
   return [expression]
```
By default, parameters have a positional behavior and you need to inform them in the same order that they were defined. e.g., look at the this function which takes in a string as input parameter and prints in on screen.
```
def printString( str ):
   "This prints a passed string into this function"
   print str
   return
```
### Calling a Function

Once the basic structure of a function is finalized, you can execute it by calling it from another function or directly from the Python prompt. Following is the example to call printString() function
```
#!/usr/bin/python

# Function definition
def printString( str ):
   "This prints a passed string into this function"
   print str
   return

# Call printStringfunction with some string as input argument
printme("Calling the user defined function!")
printme("Second call to the same function")
```

Above code will print 
```
Calling the user defined function!
Second call to the same function
```
[Lesson: Declaring and Using functions](https://github.com/learn-co-curriculum/python-defining-functions-readme)

[Lab: Decraling and Using Functions ](https://github.com/learn-co-curriculum/introduction-to-functions-lab
)
### Scope of Variables:


Scope refers to the visibility of variables. In other words, which parts of your program can see or use it. Normally, every variable has a global scope. Once defined, every part of your program can access a variable.

It is very useful to be able to limit a variable's scope to a single function. In other words, the variable wil have a limited scope. This way, changes inside the function can't affect the main program in unexpected ways

[Lesson: Scope of a variable](https://github.com/learn-co-curriculum/python-scope-readme)

Just to make things clear: Variables don't have to be and can't be declared in the way they are declared in programming languages like Java or C. Variables in Python are implicitly declared by defining them, i.e. the first time you assign a value to a variable, this variable is declared and has automatically the data type of the object which has to be assigned to it. If you have problems understanding this, please consult our chapter about data types and variables, see links on the left side.

### Function Arguments:


Virtually every programming language has functions , a way of separating out a block of code that can be called many times from different places in your program, and a way to pass parameters into them. Python is no different, so we'll quickly run over the standard stuff that most languages have, then take a look at some of the cool stuff Python has to offer.

[Lesson: Arguments to a Python function](https://github.com/learn-co-curriculum/function-arguments-readme)

[Lab: Arguments to a Python function](http://github.com/learn-co-curriculum/function-arguments-lab)

### Coding Lab: Creating a simple calculator
This lab will allow you to combine the programming skills and ideas that you have gathered upto this point including iterations, conditionals, datatypes, user I/O and functions. [Click here]() to access the lab. 

### Summary and Conclusion: 
In this lesson we saw how functions can be used as an effective method to re-use code repeatedly by passing different parameters under same processing logic. We learnt how to create new functions, call them from main program body ( or other functions), pass on values as parameters to the functions. We also looked at scoping variables for defining variables at global and local level and discussed the applications of this feature. The lesson concluded by asking students to develop a simple calculator in Python by combining all the coding skills that students have learnt upto this point in their course. 

### Useful Links 

http://introtopython.org/introducing_functions.html

https://en.wikibooks.org/wiki/A_Beginner%27s_Python_Tutorial/Functions

https://matthew-brett.github.io/teaching/global_scope.html

https://www.python-course.eu/python3_global_vs_local_variables.php

https://www.pythoncentral.io/fun-with-python-function-parameters/

https://www.programiz.com/python-programming/function-argument
