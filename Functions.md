### Python Functions

A Function is a block of code, that is meant to be reused and perform a single specific purpose. Functions make a more module oriented application.

## How to define a Function in Python

    * Start with the keyword 'def'.
    * Followed by the function name.
    * Then parenthesis '()'
    * Within the parenthesis you can add/define all needed arguments, this is optional
    * After that you put a colon ':' and after this all lines within the function should be indented
    * After that you can optionally add a description of what the function does, it should be a string within quotation marks.
    * Then you write the block of code of the function
    * And last you use the keyword 'return' to exit the function, optionally you can return a statement to the caller.

## Example Function in Python

ddef addnumbers(num1,num2):
"This function add two numbers and then returns the result"
result = num1 + num2
return result

print(addnumbers())

## Types of Arguments we can pass in a Function

    * Required or Positional Arguments
    * Keyword Arguments
    * Default Arguments
    * Variable length Arguments

### Types of Functions

    * User Defined Functions
    * Build-in Functions
    * Anonymous Functions

## Required or Positional Arguments

    These are the most common type of arguments, we have to pass the arguments in correct positional order. The number of arguments when we call the function
    must match the number of arguments of the function definition.

    Example:

    def addnumbers(num1,num2):
        "This function add two numbers and then returns the result"
        result = num1 + num2
        return result

    num1 = 10
    num2 = 5
    print(addnumbers(num1,num2))

## Keyword Arguments

    when we use the name of the argument when passing the values during the call of a function. In this case the order of the arguments doesn't matter.

    Example:

    def addnumbers(num1,num2):
        "This function add two numbers and then returns the result"
        result = num1 + num2
        return result

    print(addnumbers(num2=10, num1=5))

## Default Arguments

    We use this when defining a function, we set a default value in case the caller of the function doesn't provide one.

    Example:

    def addnumbers(num1,num2=5):
        "This function add two numbers and then returns the result"
        result = num1 + num2
        return result

    num1 = 10
    print(addnumbers(num1))

## Variable-length Arguments

    This is when we sometimes pass more arguments than the ones defined in the function.

    def printnumbers(num1,*nums):
        "This function add two numbers and then returns the result"
        print(num1)
        for num in nums:
            print(num)
        return

    num1 = 10
    print(printnumbers(num1,20,30,40))

# User-made functions

    These are the main focus of the workshop and are the functions that we will make to solve a specific single purpose of our program.

## Python Build-in functions

    The built-in Python functions are pre-defined by the python interpreter. There are over 60 built-in python functions. These functions perform a specific task and can be used in any program, depending on the requirement of the user.

    Examples:
    print()
    input()
    round()
    abs()
    float()
    int()
    str()

## Anonymous Functions

    These functions are called anonymous because they are not declared or defines in the normal way. instead of using the keyword def, we use the keyword lambda.

    Example:

    sum = lambda num1,num2: num1 + num2
    print(sum(10,20))

## Scope of the variables

All denied variables defined in the body of a function have a local scope, and this means that these variables can only be accessed inside the function they are declared, in the contrary all variables declared outside function in the program body have a global scope, they can be access at any point in the body of the program and also by all the functions.
