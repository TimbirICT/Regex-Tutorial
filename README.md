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
Character classes (\d, \w) match symbols from character sets. In this URL regex, \d matches digits, and \w matches letters, digits, and underscores.

### Flags
Regex flags, such as multiline (m) and global (g), impact the search. Multiline affects the use of '^' and '$' anchors, while global returns all matches.

### Grouping and Capturing
Grouping is achieved by wrapping portions in parentheses. Captured groups allow applying quantifiers and facilitate referencing specific parts.

### Bracket Expressions
Bracket expressions ([...]) define sets of characters. Special characters within, like ^, ., or /, are escaped with a backslash () to match them literally.

### Greedy and Lazy Match
Greedy matches (default) attempt to match as much as possible. Lazy matches, achieved by adding ?, match the shortest possible string. Greedy is usually preferred for URL regex to ensure comprehensive matching.

### Boundaries

### Back-references
Back-references in regular expressions allow referencing and reusing previously captured groups within the expression. They are denoted by \1, \2, and so on, representing the first, second, and subsequent captured groups. However, in the provided URL regex, back-references are not explicitly utilized. Back-references become particularly useful when validating patterns with repeated structures, such as HTML tags.

### Look-ahead and Look-behind
Look-ahead and look-behind assertions in regular expressions are used to assert that a certain pattern is (or is not) present ahead or behind the current matching position, without including it in the match itself. These assertions help refine pattern matching based on context.

Look-ahead '((?=...)' and '(?!...))': Look-ahead assertions check if a pattern is ahead of the current position without consuming characters. For instance, (?=https) in the URL regex ensures that the URL starts with "http" or "https" without including it in the match.

Look-behind '((?<=...)' and '(?<!...))': Look-behind assertions check if a pattern exists behind the current position without consuming characters. In the URL regex, look-behind is not explicitly used.

## Author

Timbir Middlebrooks is a student of Web Development with the University of Kansas' online coding bootcamp. To see more of his work visit his github profile at https://www.github.com/TimbirICT.

You can also email him at tmiddlebrooks99@gmail.com