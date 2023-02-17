# Regex Tutorial

Regular expressions or Regex expressions are patterns used to match character combinations in strings. In JavaScript, regex expressions are also objects. This tutorial will use a regex expression to check if a URL is valid.

## Summary

This tutorial will break down the following regex expression ```/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/``` into its components. This regex expression will solve if the input is a valid URL.

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

### Anchors

Anchors have a special meaning in regular expressions. They do not match any character. Instead, they match a position before or after characters:
  - `^` – The caret anchor matches the beginning of the text.
  - `$` – The dollar anchor matches the end of the text.

In this example ```/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/```:
  - The `^` is initializing the start of our text at the next index
  - The `$` is concluding the end of our text and the index before it
  So after this component we have ```(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?```

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Author

This tutorial was created by [Anthony Frederick](https://github.com/AnthonyFrederick7)
