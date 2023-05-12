# Regex

Regular expressions (regex) is a remarkably versatile tool for pattern matching and string manipulation in JavaScript. By defining a search pattern as a sequence of characters, regex can match, replace, or extract specific parts of a string, facilitating a wide range of complex string manipulation tasks. In JavaScript, these patterns are represented by the RegExp object, which provides an array of methods for working with strings. Whether it's validating user input, searching and replacing text, or extracting data from a string, regex in JavaScript offer extensive pattern matching functionality, including character classes, repetition, grouping, and much more.

## Summary

In this content you will find a guide to all aspects of Regex. This table of contents can be used as a roadmap to navigate through the intricacies of pattern matching.

It will review various topics, including anchors, quantifiers, OR operators, character classes, flags, grouping and capturing, bracket expressions, greedy and lazy matching, boundaries, back-references, and look-ahead and look-behind assertions.

Here is an example of a regular expression in JavaScript that matches all email addresses:

```
const emailRegex = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;
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

### Anchors

In the world of regular expressions, "Anchors" play a critical role. Just like anchors secure a ship in place, regex anchors help to define the position of a pattern within a string.

In JavaScript, there are two types of anchors: the caret ^ and the dollar sign $. 

For example, the pattern /^hello/ will match the word "hello" only if it appears at the beginning of a string. Similarly, the pattern /world$/ will match the word "world" only if it appears at the end of a string

### Quantifiers

There are several types of quantifiers. The most common ones are:

The asterisk (*) matches zero or more occurrences of the preceding pattern.
The plus sign (+) matches one or more occurrences of the preceding pattern.
The question mark (?) matches zero or one occurrence of the preceding pattern.
Curly braces ({}) allow you to specify the exact number of occurrences of the preceding pattern.

Quantifiers are essential for creating flexible and dynamic pattern matching expressions. By using quantifiers in combination with other regex syntax, you can create complex and sophisticated pattern matching logic.

### OR Operator

With OR operators, we can combine and match multiple patterns in a single regex expression.

The OR operator is represented by the vertical bar (|) character. It's like a fork in the road - we can choose one path or the other, depending on which pattern occurs first in the string.

So check this out - the pattern /hello|world/ is like having a choice between saying "hello" or "world" - you can't go wrong with either one! Plus, the OR operator can be used in combination with other regex syntax, like character classes and quantifiers, to really beef up your pattern matching skills.

### Character Classes

a Character Class is a set of characters that you want to match in a string. It's like saying, "Hey, I'm looking for any of these specific characters, and I don't want anything else." You can use Character Classes to match letters, numbers, symbols, or even specific ranges of characters.

Character Classes are denoted by enclosing the set of characters in square brackets ([]). So, for example, the pattern /[aeiou]/ would match any vowel in a string.

But wait, it gets even better! You can use special shorthand codes to match common Character Classes, like digits (\d), letters (\w), or whitespace (\s). And if you want to match any character except those in your Character Class, you can use the caret (^) symbol at the beginning of the brackets.

### Flags

Flags are special parameters that you can add to a regex pattern to modify its behavior. They can control things like case sensitivity, global matching, and whether the pattern should match across multiple lines.

There are several flags that you can use with regex patterns. The most commonly used flags are:

i (case insensitive) - Matches regardless of case sensitivity
g (global) - Matches all occurrences in a string, not just the first one
m (multiline) - Matches across multiple lines, not just the first line

You can add flags to a regex pattern by placing them after the closing slash (/) of the pattern.

### Grouping and Capturing

Grouping allows you to create sub-expressions within your regex pattern, which can then be captured and used in your code. This can be incredibly useful for extracting specific pieces of information from a string, or for manipulating text in complex ways.

you can use parentheses () to group sub-expressions within a regex pattern. For example, the pattern /(hello)+/ would match "hello", "hellohello", "hellohellohello", and so on. The + after the parentheses means "one or more", so it's matching any number of repetitions of "hello".

Capturing allows you to extract the values matched by your sub-expressions and use them in your code. You can reference captured groups by number, starting with 1 for the first group. For example, if you have the pattern /(\d{3})-(\d{3})-(\d{4})/ to match a phone number in the format XXX-XXX-XXXX, you can reference the captured groups as $1, $2, and $3 in your code.

### Bracket Expressions

Bracket expressions are a way to match a specific set of characters or a range of characters in a string using square brackets.

### Greedy and Lazy Match

In regex, "greedy" and "lazy" matching are two ways of finding matches in a string. Greedy matches try to match as much as possible, while lazy matches try to match the shortest possible string that fits the pattern. 

### Boundaries

boundaries are used to define the start or end of a word or line. They allow you to match patterns only at specific positions in the string, such as the beginning or end of a line or word. The most common boundary characters are the caret (^), which matches the beginning of a string or line, and the dollar sign ($), which matches the end of a string or line. 

### Back-references

Back-references are a feature in regular expressions that allow you to match a previously captured group within the same regular expression. A back-reference refers to a previous capturing group and allows you to reuse that captured value in a subsequent part of the regular expression.

### Look-ahead and Look-behind

Look-ahead allows you to check if a pattern exists after the current position without actually including it in the match. Look-behind allows you to check if a pattern exists before the current position.

Both look-ahead and look-behind are denoted by special syntax. Look-ahead is denoted by "(?=pattern)" for positive look-ahead or "(?!pattern)" for negative look-ahead, while look-behind is denoted by "(?<=pattern)" for positive look-behind or "(?<!pattern)" for negative look-behind.

## Author

In the pursuit of success, it is important to be well-prepared, have a clear vision, and be ready to seize opportunities when they arise. My own success at a young age was not due to mere luck, but rather the result of putting in the necessary time and effort to prepare for and capitalize on opportunities. Drawing on my ten years of experience in high-level business, I am able to chart a course for success. In addition to my professional endeavors, I also prioritize my roles as a father to my beloved daughter and a husband to my better half. By balancing work, family, and ongoing education - I am currently pursuing studies in web development at UCF - I am able to continue moving forward on a path of growth and achievement.


Austin David Nobregas

(https://github.com/Anobregas)



