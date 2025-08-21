# Multiple Function Calculator
## Description

A Java program that calculates different mathematical functions based on the input value of x. The program uses a piecewise function with three distinct mathematical operations depending on the range of the input value.
Function Definition

The program implements the following piecewise function:
text

f(x) = {
  x² + 1      if x ≤ 0
  1/x²        if 0 < x < 1
  x² - 1      if x ≥ 1
}

How to Use
Prerequisites

    Java Development Kit (JDK) installed on your system

    Basic knowledge of running Java programs from command line or IDE

Running the Program

    Compile the Java file:
    bash

javac MultipleFunction.java

Run the compiled program:
bash

    java MultipleFunction

    Input:

        The program will wait for you to enter a decimal number (double)

        Enter your value for x and press Enter

    Output:

        The program will calculate and display the result based on the piecewise function

Example Usage
text

Input: -2.5
Output: 7.25

Input: 0.5
Output: 4.0

Input: 2.0
Output: 3.0

Code Structure
Main Class: MultipleFunction

    Contains the main method that handles user input and output

    Reads a double value from standard input

    Calls the f(x) function and prints the result

Methods:

    f(double x) - Main dispatcher function

        Determines which sub-function to call based on the value of x

        Returns the computed result

    f1(double x) - Handles x ≤ 0

        Computes: x² + 1

    f2(double x) - Handles 0 < x < 1

        Computes: 1/x²

    f3(double x) - Handles x ≥ 1

        Computes: x² - 1

Error Handling

    The program uses simple conditional logic without explicit error handling

    Invalid inputs (non-numeric values) will cause the program to throw exceptions

    Division by zero is avoided since f2 is only called when 0 < x < 1

Notes

    The program uses double precision floating-point arithmetic

    All mathematical operations follow standard Java arithmetic rules

    The program terminates after calculating and displaying one result

Author

Java program implementing a piecewise mathematical function calculator.
