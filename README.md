# CS-regex

Regular expressions are used to compare or find patterns of characters in a string. They (regular expressions) may also be used to find and replace a character or sequence of characters within a string. Commonly, developer's are introduced to regular expressions as a form of validation for user input.  

## Summary
 This file will analyze the regex expression:

 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
 
 In this scenario, the regex is used to match the character information for a valid e-mail address.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

In the expression, the anchors used are (^) at the beginning of the expression and ($) at the end.

### Quantifiers

The expression uses a greedy quantifier method, by using the (+) symbol to concat multiple patterns or sequences to be compared to the input. By placing the {min, max} values of {2,6} the expression specifies that the input should be a minimum of 2 characters and a maximum of 6 characters.


### Character Classes

The expression uses (/d), as a reference to Javascript, to classify the use of any digit from 0 to 9.


### Grouping and Capturing 

The expression can be broken down into 3 components. First, [a-z0-9_\.-], capturing the username part of the e-mail account. Second [\da-z\.-], capturing the domain name of the e-mail server used. Third [a-z\.]{2,6}, capturing the domain extension of the e-mail server. 

### Bracket Expressions

The Bracket Expressions in this example are used to define the grouping in the expression. The brackets identifies what information should be matched with the user input. The brackets also make it easier to understand the process of data comparison. 

Bracket set 1 [a-z0-9_\.-]: includes case sensitive characters from a-z, numbers from 0-9 and underscore, periods and hyphens.

Bracket set 2 [\da-z\.-]: includes all digits, case sensitive characters from a-z, periods and hyphens.

Bracket set 3 [a-z\.]: includes case sensitive characters from a-z, periods and hyphens.

### Greedy Match

This expression uses the greedy quantifiers + and {}. By using these quantifiers, the expression is expanded to the necessary length to check all the components of an e-mail rather than having repetitive or unnecessary code.

## Author

My name is Silvia Trejo, and I have learnt to enjoy debugging.

Please checkout my github repositories: [https://github.com/sytrejo](https://github.com/sytrejo)