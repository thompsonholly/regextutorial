# Regex Tutorial

This is a tutorial about Regular expressions, or regex for short. Regex is a very useful programming tool that helps developers to solve problems. A regular expression is a pattern of one or more character literals, operators, or constructs. It helps developers do things like find and replace text, verify that input data follows the format required, and and other similar things.

## Summary

This tutorial of regex will explain the matching an HTML Tag regex. This will also explain the different components that make up a regex and how each one is used in this particular expression.

* Matching an HTML Tag: `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`

AN HTML tag contains < and > as an opening and closing "tag". An example of an HTML as viewed in source code for a webpage is: <HTML>, <main>, <div>, and so forth.

A closing tag must follow an opening tag in order to contain the code within it. If not it will not be properly run. HTML tags are not always quite as simple as the prior example and can include various specific parts through which, when run, can deploy unique tasks. Consider the following:

(MDN RegEx)[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp]



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
The characters ^ and $ are where to define the search parameters. Anything after ^ (caret) and before $ (dollar) are part of the search. 

^abc123$

The caret, ^, identifies the beginning of our string the position. The dollar, $, it identifies the end of our search string.

The anchors help the system running the search parameter to identify < and > characters with anything listed between as an alpha-numeric or special character combination.


### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

Holly Thompson is currently a full-time student in the EdEx Full Stack Coding Bootcamp at the University of Minnesota, she is the author of this Regex Tutorial. Link to GitHub profile: https://github.com/thompsonholly

