# Using URL's with Regular Expressions

This tutorial will show you how to use and implement URL's with regular expressions. Regex is a very useful way to match patterns to text, which can help you by identifying 
and extracting URL's from a given source.

## Summary

For this tutorial, we'll be looking at a pattern used for extracting URL's. 
Here is what this pattern looks like: '/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/'
This line of code will help identify what to look for in expression form. In this case, it will look for and identify URL's.

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
Anchors act as an indicator for where text starts, and ends in the expression. 

In this pattern, '^' anchors the regex at the beginning of the string. '$' anchors the regex at the end of the string. 
It acts as an identifier for a start and finish of a pattern.



### Quantifiers
Quantifiers are used to specify the number of occurrences of a character, or group. 

In our example, we use the quantifier '*' to indicate that the expression allows
for zero or more occurrences of the characters within the square brackets. 

Another quantifier used in our experession is '?'.
'?' indicates that the expression allows for zero or one occurences as opposed to zero or more.
In our expression, it indicates that the URL is allowed to have a trailing slash or not.


### OR Operator
The OR Operator allows the pattern to match with 'http', 'https', or 'ftp'.

In this expression, the OR operator we used is the '|' symbol. 

### Character Classes
Character classes are represented by square brackets, and help match a character from a character set.
In our expression, we use


### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)