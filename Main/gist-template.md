# Regex Tutorial: Matches a US ZIP code

A tutorial that comprehensively explains how a specific regular expression (regex) works by breaking down each component of the expression and detailing its function.

## Summary

The regular expression (regex) for matching a US ZIP Code can handle both the standard 5-digit format and the extended 9-digit format (ZIP+4) which includes a hyphen. Here's a regex that matches both formats:

`^\d{5}(-\d{4})?$`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components ~

Regular expressions (regex) are composed of various components that allow you to define patterns for matching strings. Here are the key components used in the regular expression (regex) for matching a US ZIP Code:

### Anchors

Are special characters used to specify the position within the string where a match should occur. Anchors don't match any characters themselves but instead represent a position in the string.

In this regex, the `^` anchor denotes the start of the string, and the `$` anchor denotes the end of the string.

### Quantifiers

Allow you to specify how many times a particular pattern should occur in the string.

In this regex,`{5}` ensures exactly five digits, and `{4}`ensures exactly four digits after the hyphen, if it exists. The `?` quantifier makes the hyphen and four digits group optional.

### Grouping Constructs

The grouping construct `( )` allows you to treat multiple tokens as a single unit.

In this regex, it's used to group the hyphen `-` with the following four digits `\d{4}`. This grouping ensures that the hyphen and the four digits are treated as one unit when applying quantifiers or making the entire group optional with the `?` quantifier.

### Character Classes

Character classes are used to specify a set of characters from which you want to match one character.

In this regex,`\d` represents a character class matching any digit from 0 to 9, while `-` matches the hyphen character literally.

### Character Escapes

Are used to match special characters or characters with special meanings as literals.

In this regex, the backslash `\` is used to escape the `d`, turning it into a special character representing a digit. This allows the regex engine to recognize it as a digit rather than the literal character "d".

## About the Author ~

Anthony Wiggins Jr is a junior software developer with a passion for coding and technology. With a background in full stack coding and hands-on experience in web development, Anthony is skilled in various programming languages and frameworks, including HTML, CSS, JavaScript, and React. He has a keen interest in creating efficient, user-friendly applications and enjoys tackling challenging problems to continuously improve his skills. His enthusiasm for learning and dedication to the craft make him a promising and valuable member of any development team.

GitHub Profile ~ [https://github.com/awigginsjr](https://github.com/awigginsjr)

GitHub Gist ~ [https://gist.github.com/awigginsjr/8767ed410ab85dedc9ce2b614adb34e0](https://gist.github.com/awigginsjr/8767ed410ab85dedc9ce2b614adb34e0)

My site is live at ~ [https://awigginsjr.github.io/17-Regex-Tutorial/](https://awigginsjr.github.io/17-Regex-Tutorial/)
