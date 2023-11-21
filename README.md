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
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
The characters `^` and `$` are where to define the search parameters. Anything after `^` (caret) and before `$` (dollar) are part of the search. 

`^abc123$`

The caret, `^`, identifies the beginning of our string the position. The dollar, `$`, it identifies the end of our search string.

The anchors help the system running the search parameter to identify `<` and `>` characters with anything listed between as an alpha-numeric or special character combination.


### Quantifiers
Quantifiers in regex are used to determind where the preceding string must be matched a pre-set number of times or more. A quantifier can be labeled as being greedy or lazy.

The `+` quantifier states that the search must match one or more of the characters set in the algorithm, characters placed to the left of the `+ are expected to match at least once:
Example: `cars+` the `+` ONLY applies to the `s` in cars. 

The `*` quantifier states that the search must match 0 or more times

The `?` quantifier states that the search must match 0 or 1 times but it is also optional.
When it is implemented this `?` makes the quantifier before it considered lazy. This allows it to match as few times as possible. The default quantifiers tend to lean towards matching as many characters as possible and are considered greedy.


`{7,9}` This is set to allow only between seven and nine characters long.


`abc|cba` This results in a match of `abc` OR `cba` only.

### Grouping Constructs
`(hijk){4}` If it a selective pattern, they are set between parentheses and include a numeric counter besides it. This example would search for the match of `abcabcabc` because the first group was denoted as `(hij)` and we included the need for it to repeat three times as `{4}`.

If there is non parentheses groups, the regex would look similarly `(?:hijk){4}` or `(?:HIJK`.

### Bracket Expressions
A regex captured in square brackets is meant to match a single character or collating element.  An example is `[a-z]` as a bracket expression.

### The OR Operator
The `|` operator acts like a Boolean OR. It matches the expression before or after the `|` and can be utilized inside a group or in  a whole expression. It causes the search-string to seek a match of either what is before or follows the `|`. 
In the example: `<hijk>|<kjih>` it is looking for either `<hijk>` or `<kjih>`.

### Flags
Expression flags are used after the initial closing forward slash expression.

The `i` ignores case

The `g` finds all matches instead of stopping after the first match.  The `i` modifier can combine with the `g` modifier to help with the global match, if there is a case-sensitive match. 

The `m` is a flag used to match the start and end of a line instead of the start and end of a whole string. The anchors used at the beginning and end `^` and `$` of the search.

The `s` searches for whitespace characters within a string.

### Character Escapes

## Author

Holly Thompson is currently a full-time student in the EdEx Full Stack Coding Bootcamp at the University of Minnesota, she is the author of this Regex Tutorial. Link to GitHub profile: https://github.com/thompsonholly

