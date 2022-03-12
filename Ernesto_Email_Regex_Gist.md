# Email Regex Tutorial

In this tutorial I will explain the email Regular Expression commonly known as a regex. The email regex is one of the most used in programming due to its prevalence in todays society

## Summary

In short an email regex can be used to ensure an email entry is properly given by a user. I will go through its components and explain how it works as a whole. This is a email regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

-   [Anchors](#anchors)
-   [Quantifiers](#quantifiers)
-   [Grouping Constructs](#grouping-constructs)
-   [Bracket Expressions](#bracket-expressions)
-   [Character Classes](#character-classes)
-   [The OR Operator](#the-or-operator)
-   [Flags](#flags)
-   [Character Escapes](#character-escapes)

## Regex Components

### Anchors

`/^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`$/`
These refer to the first and last parts of the regex. ^ and $ resp. Which represent the beginning and ending of the regex expression.

### Quantifiers

Quantifiers are used to express how many characters are expected in a user imput email. In our email regex we have + which symbolizes that we are expecting the characters in the brackets before the plus to appear. So we expect characters a-z also numbers 0-9. The regex also has {2,6} quantifiers which translates too expecting at least two characters but up to six for our email root end; for example .ca is okay and a root ending up to 6 characters. The question mark (?) symbolizes a boolean match or no match result.

### Grouping Constructs

Regular () symbolizes a single group so we can apply criteria appropriately to that particular part of a regex. For this email regex we see we have three grouping constructs (A)@(B).(C) and thus we can verify each group with varying criteria.

### Bracket Expressions

The bracket expression symbolizes the beginning of a character class.

### Character Classes

Character classes symbolize what we can accept an imput within the scope of whatever we state within. For example in our email our first character class states we can accept any letter a-z but also any number 0-9. In contrast to the ending character class where we are only accepting a-z. Which matches emails format as there is never numbers in the end of an email.

### The OR Operator

Symbolized as a |. It states that we are matching either or. For example ([a-f0-9]{4}`|`[a-f0-9]{2}) states we are matching either 4 or two characters in a given input.

### Flags

These are optional parameters that can make the regex engine search in a different way. For example the i flag makes the entire expresstion insensitive to case. Upper or lower case characters.

## Author

Ernesto Sanchez [GitHub Profile](https://github.com/ernestosanchezCS)
Junior Developer, with a ton of drive to learn as much as possible.
