# Dart-calculator
Simple Dart calculator for use in a CLI

Related to the Medium article: *Building a Simple CLI Calculator App in Dart*

## Overview

This application allows basic calculator functionality when run from a CLI. Recursion is used to continue functionality, and the user is allowed to exit at anytime via simply typing exit.

The calculator can add, subtract, multiply, expontentiate, and divide.

## Setup and Rationale

All numerical inputs are of the `double` datatype as I wanted to account for the possiblity of decimal numbers.
The first number received is the one that has operations performed on it (i.e. it is subtracted from, divided from.)

To give myself a little variety, I used Math.pow for the exponentiation function. It will just raise the first number by the second number. Additionally, typecasting is used to account for large numbers

To receive inputs, Scanner is used. A check for the word 'exit' is first performed, and if not, the input is converted to a double.
This means, however, there is the possibility for an error if the user types in other non-numerical characters (See Future Considerations)

## Future Considerations

The incorporation of regular expressions to verify inputs would be a great improvement to this app and can be solved by 
the Pattern and Matcher classes. However, I didn't want to incorporate them at this point as this repo's purpose is to be used
as a guide to those new to Dart. 