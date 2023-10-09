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

Quantifiers are used to identify certain patterns or characters.

`*` will match 0 or more of the preceding pattern. The regex `/lu*/` will recognise the 'lu' in luan and the 'llu' in illustrates.

`+` will match 1 or more of the preceding pattern. The regex `/lu+/` will recognise the 'lu' in luan and the 'lu' in illustrates.

`?` denotes an optional marker that will match 0 or 1. Anything preceding the ? will be optional in the search. Thus the regex `/te?/` will recognise the 'tt' in https, the first 't' and the 'te' in illustrates.

`{}` curly braces will allow for minimum and maximum match cases.

> where `{a}` equals the number of instances exactly, `{a,}` matches the instances at minimum and `{a, b}` will match between the specified range.

### Character Classes

Characters can be distinguished with specific classifiers.

`\.` will match anything specified. `/.t/` will highlight the 'ht', 'st' and 'at' of the example URL.

`\d` will match a digit equivalent to '0-9'. None in this case.

`\w` will match any alphanumeric characters equivalent to 'a-z', 'A-Z' and '0-9'.

`\s` will match whitespace characters (spaces, tabs and line breaks).

We also have the inverse capitals of the listed classifiers.

`\D` will match any character that is not a digit.

`\W` will match any character that is not a word character.

`\S` will match any character that is not a whitespace character.

### Flags

Flags would normally act as a set of filters, but as a URL has limited parameters to set, we won't cover this.

### OR Operator

Or operators, denoted by `|`, search in a boolean fashion in which that the search will take into account the specified expressions.

Our example `(.com|.net)` will search for the domain used, which will be '.com' in this case.

### Grouping and Capturing

We can take a broader look at the whole string and encapsulate certain patterns with grouping, using the parentheses `()`. Anything inside the parentheses will be in its own group and act in a targeted manner. Not too prevalent in our case here.

### Bracket Expressions

Similar to Or operators, bracket expressions accept the parameters set inside the `[]`. Utilising all the properties laid out before, we can combine them all in a single bracket expression.

Small example of this would be `[a-l]`. This will match the range from 'a' to 'l' in the lowercase capacity.

### Greedy and Lazy Match

By default, quantifiers are greedy in which that they will match as many characters as possible (think of the `*` or `{}`). On the other hand, we have the lazy, best represented by the `?`. This acts in the opposite nature and will match the least.

## Author

Written by Luan. For more works, visit:

<a href="https://github.com/luanillustrates">Luan Illustrates Github</a>
