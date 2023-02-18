# Regex Tutorial

Regular expressions or Regex expressions are patterns used to match character combinations in strings. In JavaScript, regex expressions are also objects. This tutorial will breakdown a regex expression to check if a URL is valid.

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

Anchors have a special meaning in regular expressions. There are 2 anchors, they do not match any character. Instead, they match a position before or after characters:
  - `^` – The caret anchor matches the beginning of the text.
  - `$` – The dollar anchor matches the end of the text.

In our regex expression ```/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/```, we can see the scope of our input between the anchors which is ```(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?```

We can test a simple regex expression with anchors by this example:

```
let website = 'https://github.com';
console.log(/^(https)/.test(website));
console.log(/(.com)$/.test(website));
```

Both console.logs will be `true` because the `/^(https)/` will match any text that starts with the letters `https` and `/(.com)$/` will match any text that ends with the letters `.com`.

### Quantifiers

Quantifiers match a number of instances of a character, group, or character class in a string.

Our regex expression has FOUR types of Quantifiers.

1. The range `{n, m}`
  - The range matches a character or character class from `n` to `m` times.
  - `{2,6}` in our regex epression is allowing `[a-z\.]` to have 2 to 6 characters in length.

2. The Shorthand `+`
  - `+` is short for `{1,}`. It will search from the first index to last inside its capture.
  - `+` in our regex expression is allowing `[\da-z\.-]` to have any amount of characters from 1 to unlimited.

3. The Shorthand `?`
  - `?` means zero or one. It is the same as `{0,1}`.
  - `https?`, `(https?:\/\/)?`, and `/?` is using the `?` quantifier to allow the text to not exist or to exist ONCE.

4. The Shorthand `*`
  - The quantifier `*` means zero or more. It is the same as `{0,}`.
  - `[\/\w \.-]*` and `([\/\w \.-]*)*` is using the `*` quantifier to allow the text to not exist or to exist an unlimited amount of times.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Author

This tutorial was created by [Anthony Frederick](https://github.com/AnthonyFrederick7)
