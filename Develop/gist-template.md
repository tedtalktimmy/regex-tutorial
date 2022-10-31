# regex tutorial

This is a tutorial breaking down and explainings the specifics of a regular expression to understand what its use/purpose is.

## Summary


A regular expression (regex) is a a sequence of characters that defines a search pattern.  The snippet below shows the particular regex I will be breaking down.

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```


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
There are three elements in this regex:
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```


  - ***element No.1 -*** USERNAME
  ```
  ([a-z0-9_\.-]+)
  ```

This checks the portion of email address to match username.  This cannot contain special characters. snippet below provides an example of the special characters not allowed. Please note: underscores and dashes do not fall in this criteria and can be used.

  ```
  %, &, ?, $, etc. etc.
  ```

  - ***element no.2 -*** DOMAIN
  ```
  ([\da-z\.-]+)
  ```
This checks the domain part of the email address to match. This can only contain letters, numbers and/or dashes.

- ***element no.3 -*** SUFFIX
```
([a-z\.]{2,6})
```
This checks the suffix of the email address. ("gmail.com" and "outlook.com" are examples of a email suffix). The last digits, {2,6}, determines the shortest and longest a suffix can be.



### Anchors
^ and $ are examples of anchors.  ^ defines the beginning of a string, while $ defines the end of a string (i.e ^qwerty$).


### Quantifiers
Examples of quantifiers are as follows: ```+```  ,  ```{x,y}```


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

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
