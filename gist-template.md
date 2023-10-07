# RegEx tutorial - matching a URL

This tutorial is an explanation of regular expression and its patterns used to describe, match or parse text character combinations in strings.
In this tutorial, we will be examining the regular expression to match a URL and breakdown the various components that comprise regex. Our example url will be

> https://www.luanillustrates.com

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

The regular expression format utilise the forward slashes as opposed to the quotation marks. Anything within these slashes will comprise the regular expression search.

```
/{regular expression}/
```

### Anchors

Anchors describe either the start of a string with `^` or the end with `$`. Looking at our example url,

a regular expression of `/^https/` and `/.com$/` will return with a match for our start and end of the string respectively.

This way, we can examine if the site is utilising a secure version of http or if the domain being used is '.com'.

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

<a href="https://github.com/luanillustrates">Luan Illustrates Github</a>
