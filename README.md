# Regex-Tutorial
We will be taking a look at Regex, what they do and how they work. Regex is also known as regular expressions.

## Summary

Regex is useful when gathering specific information in any text, it uses a special search pattern of ASCII or unicode characters.
It can manage, replace, and translate strings. Examples:

- 10-digit string starts with a 2: `2\d{9}`
- Contains {iii}: `i{3}`
- Validate email: `/[\w._%+-]+@[\w.-]+\.[a-zA-z]{2,4}/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)

## Regex Componenents

### Anchors

An anchor does not consume a string or characters, is similar to a delimiter. Sets boundaries on the work that can be accessed.

* `^` : Place at beginning of a string or line
* `$` : Place at end of a string or line

### Quantifiers

There are six types of quantifiers, each with three levels of intensity. 
* Eager: matches as much as possible and gives back 
* Reluctant: matches as much as possible and does not give back
* Possessive: match as little as possible

```
Zero or one: (E)? (R)?? (P)?+
Zero or more: (E)* (R)*? (P)*+
One or more: (E)+ (R)+? (P)++
i times: (E){i} (R){i}? (P){i}+
At least i times: (E){i,} (R){i,}? (P){i,}+
At least i, at most j times: (E){i,j} (R){i,j}? (P){i,j}+
```

### OR Operator

There are two types of OR Operators. OR Operators will return what matches the string that the two characters match.

* `a(b|c)` - Matches a string that is followed by variables b or c (inclusive)
* `a[bc]` - Matches a string that is followed by variables b or c (exclusive)

### Character Classes

Character Set will make Regex match a single character in the string, whether it be a digit, character, word, or whitespace.

```
\d matches a digit (0-9)
\w matches a character (a-z)
\s matches a whitespace (' ')
. matches a character
\D matches a non-digit character
\W matches a non-character that is a-z
\S matches a non-whitespace
```

### Flags

Flags are parameters that change the way the expression searches. There are three main Flags that are pretty straightforward.

* `g` - Global: Makes the expression searh fro all occurences
* `m` - Multi-line: Matches the start and end of a line, not whole string
* `i` - Insensitive: Makes the expression case-insensitive

## Author

### Enzo Sperduti

* [Author's GitHub]
