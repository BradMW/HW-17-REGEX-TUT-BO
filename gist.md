# HW-17-REGEX-TUT-BO

This is a REGEX tutorial explaining how the expression: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, can be used to find and match emails. This can be used while validating an email in an application

## Summary

Regular expressions are a sequence of characters that are used to define a search pattern. REGEX is a common term for these strings. They can be used in multiple ways such as searching through a document to find all phone numbers or to search for email addresses and even validate them inside of an application. An example of this is making sure that the email you enter to a login page is the same one that is kept on your profile to ensure a secure log in.

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

Anchors are used to set a defined area in your search terms. For instance, ^ is a start anchor and $ is an end anchor. These are used to set a position at the start and end of a string.

### Quantifiers

Quantifiers are used to set the search terms of the expression. the + symbol in the expression matches 1 or more to the preceding token. For example ([a-z0-9_\.-]+), this is searching for any characters matching whats in the brackets and then continuing to include them into the string with the + til there are none left to match it. An example of a quantifier in use is this: ([a-z\.]{2,6}). This is going through and looking for those characters at the end of an email and finding the ones that are between 2 and 6 charaters in length. (ex .co, .com, .org).

### Grouping Constructs

Grouping is done by using (). in this REGEX there are 3 groups that are defined. ([a-z0-9_\.-]+) searching for letters and numbers in the front of an email, ([\da-z\.-]+) searching for letters and numbers after the @, and ([a-z\.]{2,6}) looking for these characters after the . in an email. (ex "email" @ "gmail" . "com")

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
