# Class 02

## What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?

Test-Driven Development (TDD) in Python follows key principles: write a test, run the test (which should fail), write code to pass the test, and then run all tests. TDD improves code coverage, promotes simpler design, prevents regressions, detects bugs early, and serves as documentation. By following these principles, developers create higher quality code with fewer bugs and easier collaboration.

## Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?

The purpose of the `if __name__ == '__main__':` statement in Python scripts is to check if the current module is being executed as the main program. It allows code within this block to be executed only when the script is run directly, not when it is imported as a module. This conditional is useful for including test cases, running standalone scripts, or executing certain initialization code when the script is run directly.

## Describe the concept of recursion in Python:

Recursion in Python is a programming technique where a function calls itself to solve a problem. It involves breaking down a complex problem into smaller subproblems until a base case is reached. Recursion requires defining both the base case and the recursive case, allowing the function to call itself repeatedly until the desired result is obtained.

## What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs:

In Python, modules are single files containing Python code, while packages are directories containing multiple modules. To create a module, simply create a .py file with Python code. To create a package, create a directory and include an init.py file. To import and use modules/packages, use the import statement followed by the module/package name. Functions, classes, and variables within modules/packages can be accessed using dot notation.