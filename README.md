# PROGRAMMING LANGUAGE IMPLEMENTATION & PARADIGMS
LEXICAL AND SYNTAX ANAYLSIS

This is the instruction how to run the coding.

## Valid Input
Here are the valid input for the expression
- Numbers
- Variables such as **x or y**
- Operator such as **+ - * /**
- Comparison such as **< > =**
  
## Lexical Analysis
Lexical analysis is the first stage of compiler design that analyses and breaks down source code into its fundamental components called tokens. 
This is also referred to as scanning.

The program will ask for input:

````
Enter the input text:
````
Then it will generate the expression in token by their type

### Example

````
Enter the input text: 4 + 6 ;
Tokens:
Type: Number, Value: 4
Type: Operator, Value: +
Type: Number, Value: 6
Type: Punctuators, Value: ;
````

## Syntax Analysis
It verifies whether or not the input is in the proper syntax (of the language in which it was written) by analyzing its syntactical structure. 
It accomplishes this by constructing a data structure known as a syntax tree or parse tree.

The program will ask for input:

````
Enter the input text:
````
Then it will generate the tokens in parse tree.
### Example

````
Enter the input text: 4 + 6 / 7
Tokens:
Type: Number, Value: 4
Type: Operator, Value: +
Type: Number, Value: 6
Type: Operator, Value: /
Type: Number, Value: 7
Parse Tree:
        7 (Number)
    / (/)
        6 (Number)
 + (+)
    4 (Number)
````

## Test & Validation

The instruction same as Syntax Analysis. 
It examines the input string for arithmetic expressions containing numbers, identifiers, operators, and brackets. 
The main purpose of this code is to ensure that the compiler handles correct code and to provide an error message for incorrect code.

Assume the input is same as syntax analysis.

````
Expected Output: Valid parse tree representation
````
### Example for invalid input

````
Enter the input text: 5 6
Syntax Error at position 2: Operator expected
````
