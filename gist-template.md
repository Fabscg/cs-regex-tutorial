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
####  *You may think that <.+> (. means any non newline character and + means one or more) would only match the <em> and the </em>, when in reality it will be very greedy, and go from the first < to the last >. This means it will match <em>Hello World</em> instead of what you wanted.Making it lazy (<.+?>) will prevent this. By adding the ? after the +, we tell it to repeat as few times as possible, so the first > it comes across, is where we want to stop the matching.*

### Boundaries
#### *A word Boundary in most Regex dialects is a position between \w and \W (non word char), or at the beginning or end od a string if it begins or ends(respectively) with a word character ([0-9A-Za-z_]). So in the string "-12", it would match before the 1 or after the 2.*

### Back-references
#### *Are used to match the same text previously matched by a capturing group. This both helps in reusing previous parts of your pattern and ensuring two pieces of a string match. for example, if you try  to verify that a string has a digit from zero to nine, a separetor, such as hyphens, slaches or even spaces, a lower letter, another separator, the another digit from 0 to 9, you could use aregex like this.* Example:
* [0-9][-/ ][a-z][-/ ][0-9]

### Look-ahead and Look-behind
#### *For the start, let’s find the price from the string like 1 turkey costs 30€. That is: a number, followed by € sign.The syntax is: X(?=Y), it means "look for X, but match only if followed by Y". There may be any pattern instead of X and Y. for an integer number followed by €, the regexp will be \d+(?=€):*
### Look-Behind 
#### *Look-Bihind is not supported in V8 browsers, such as Safari, Internet Explorer. This is similar  but it looks behind. That is, it allows to match a pattern only if there's somehting before it* Example:
* Positive lookbehind: (?<=Y>X), matches X, but only if there is Y before it.
* Negative lookbehind: (?<!Y>)X, matches X, but only if there is no Y befor it.
* For example, let’s change the price to US dollars. The dollar sign is usually before the number, so to look for $30 we’ll use (?<=\$)\d+ – an amount preceded by $:

## Author
   Fabiola C. Gamboa
I started doing cogind in febraury 2020, I loved right away, then I got involve a lot when I got couple of books and a course on line, but it wasn't enough, specially when you are a self learner, you have so many questions but even when you googled everything you still want to know more. Then I decided to take this Bootcamp from the U of T, and It has been so helpfull for me and the way I had been learning has been amazing, when I look at in the past couple of years, I relized how much had been learning in the last 5 months. (https://github.com/Fabskickass/cs-regex-tutorial)
