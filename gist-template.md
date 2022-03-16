# Regex Tutorial

In this tutorial, I am going to explain the use of Regex (regular expressions) to match emails using expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. You can use this when validating emails usings applications like Node or MongoDB.


## Summary

A regular expression is a sequence of characters that defines a search pattern. We can use regex to find patterns within a string or validate an input, in our case an email. This tutorial will walk you through how regex works and how it applies to matching an email. 

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

The anchors used in this regex expression for matching an email are ^ , which tells us the beginning of the string and $ to tell us the ending of the string. 

### Quantifiers

The quantifiers in this regex include the + operator, which connects the users email name with their email service. Another quantifier would be {2,6}, which will allow the email range to be between 2-6 for the character set of [a-z\.].

### Grouping Constructs

Group #1 in this expression is ([a-z0-9_\.-]+), which is used to match the users email name. The second group is ([\da-z\.-]+) which is used to match the email service (ex: gmail, yahoo, etc.). Then the last group ([a-z\.]{2,6}) is used to match the .com.

### Bracket Expressions

The bracket expressions used for email matching inlcludes the character set of [a-z0-9_\.-], which will match any letter a-z in lower case only. It will also match numbers 0-9 and the characters "_", "-", and ".". 

### Character Classes

The character class in the expression is \d, which matches single characters that are numbers from 0-9. It will only match a single digit, not double or triple digit numbers.


### The OR Operator

The OR operator | matches the charcters or expression on the left or right side of the Or operator. in this regular expression an Or expression was used in the middle between /^#?([a-f0-9]{6} and [a-f0-9]{3})$ so that the expression could match either the left or right expression. With this both 6 and 3 charcter hexadecimal codes are acceptable.

## Author

My github is https://github.com/dmcarver01611
