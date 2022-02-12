# Computer-Science/Regex-Tutorial

In this tutorial I will be giving a little explentation and description of Regex. What is it and what is this for?

## Summary
Regex stands for Regular Expression. This regular expressions can be difficult to learn and memorize, but using them more often can helo you to learn some of them for your work.
They are a sequence of characters that can be use to specify a string, a text or for input valdations. An example of this that you  had already seen before is somehting like this:
" /[A-Za-z_\-]+/ "

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
#### *Anchor match a postion within a string, not character.*  To start of a string or start of line in multi-line pattern. for example: 
* ^ = Star of a String or start of line on multi-line pattern
* \A = Start of a string 
* $ = End of a string or line
* \b = Word boundary

### Quantifiers
#### *Indicate that the preceding token must be matched a certain number of time* Example:
* * = 0 or {3} exactly
* + = 1 or {3,} 3 or more

### OR Operator
#### *this is a Boolean operator which would return the value of true or boolean value of 1, if either of both of the operands are true or have Boolean value of 1.* 

### Character Classes
#### *This is the most basic regex concept after a literal match. It makes one small sequence of characters match a larger set of characters.* Example:
* [A-Z] = Culd stand for any uppercase letter in emglish alphabet
* \d = Could mean any digit
* \D = Non digit
^ \w = Word

### Flags
#### *flags means dot all. Match everything , even newlines. By default the dot match everything but the newly characters*

### Grouping and Capturing
####*Capturing forups are a way to treat multiple characters as single unit. They are created by palcing the characters to be grouped inside a ser of parentheses.* Example:
* . = Any character except new line
* (a|b) = a or b
* (...) = Group

### Bracket Expressions
#### *A Breacket Expression is a list of characters enclose by ['and']. It matches any single character in that list. If the character of the list is the caret '^', then it matches any character NOT in the list.* Example:
* [:alpha:] and [:digit:] is the same as [0-9A-Za-Z]

### Greedy and Lazy Match
#### **

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
  Fabiola C. Gamboa
  
  [Github](https://github.com/Fabskickass/cs-regex-tutorial)


