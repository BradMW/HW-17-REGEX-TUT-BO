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

Grouping is done by using (). in this REGEX there are 3 groups that are defined. ([a-z0-9_\.-]+) searching for letters and numbers in the front of an email, ([\da-z\.-]+) searching for letters and numbers after the @, and ([a-z\.]{2,6}) looking for these characters after the . in an email. (ex "email" @ "gmail" . "com").

### Bracket Expressions

This email validation REGEX has 3 bracketed expressions built into it. The first is [a-z0-9_\.-] and this will look for all characters that match whats inside the brackets. This will look for letters A-Z as well as numbers 0-9 to find what could be your username. Then ([\da-z\.-] will look for the (/d) digits and the letter range of A-Z. Finally [a-z\.] will look for the end of the email address.

### Character Classes

This is used to define a set of characters. This email validator used /d to look for the digits 0-9. and a-z to search for all letters.

### The OR Operator

The OR Operator is used to make strings match. The | is a logical operator that could be used to let the user choose to enter an email OR a phone number to validate their information in the data base.

### Flags

An example of a flag is /m. /m is a multiline flag that can be used to return matches that span multiple lines because the anchors will find and match the start and end of individual lines.

### Character Escapes

Character Escapes give characters a special meaning. \ is a special character that gives the following character a litteral meaning. For example \. is looking for a string with a . in it. (me@me "." com). This helps it validate that an email is real.

## Author

[BradMW](https://github.com/BradMW)
