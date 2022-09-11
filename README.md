# Regex

Regular Expression or Regex for short, is a sequence of character, that defines search pattern for text.

## Summary

Regular expressions are patterns used to match character combinations in strings. In JavaScript, regular expressions are also objects.
Below are a number of commonly used regex components, with their definitions and examples.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Author](#author)
- [References](#references)


<br>

## Regex Components

Regex is considered literal. Most characters stand for themselves. The pattern must be wrapped in slash characters (/).
Certain characters however, called Metacharacters, have special meaning and must be escaped with (\) if to be used as characters.  


<br>

### <strong>Anchors</strong>

Anchors cause a match to succed or fail depending on the current position in the string, but they do not cause the engine to advance through the string or consume characters. 
Metacharacters are used to act as anchor for the regex. 

Example: 

- <strong>^</strong> signifies a string that begins with characters that follow it.

- <strong>$</strong> signifies a string that ends with characters that precede it.


<br>

### <strong>Quantifiers </strong>

Quantifiers set limit of the string that regex matches. Minimum / maximum number of characters regex is looking for.

Example:

- <strong>*</strong> matches pattern 0 or more times.
- <strong>+</strong> matches pattern 1 or more times.
- <strong>?</strong> matches pattern 0 or 1 time.
- <strong>{}</strong> provides 3 different ways to set limit for a match:
    - { n } matches n number of times.
    - { n, } matches at least n number of times.
    - { n, x } matches from minimum of n to maximum of x number of times.


<br>

### <strong>Grouping Constructs</strong>

It means to break into sections; and a way to it is by using parentheses (())
Each section within parantheses is known as subexpression.

Example: <strong>(abc) : (def)</strong>.

Grouping Constructs have 2 primary categories, Capturing and Non-Capturing.

Capturing groups capture the matched character sequences for possible re-use. Non-Capturing do not. 


<br>

### <strong>Bracket Expressions</strong>

Anything inside a set of square brackets ([]) represents a range of characters that we want to match. 

Example: 

- <strong>[abc]</strong> - will look for <strong>a</strong> or <strong>b</strong> or <strong>c</strong>.
- <strong>[a-z]</strong> - will look for will look for any lowercase <strong>a</strong> to <strong>z</strong>.
- <strong>[0-9]</strong> - will look for any number between <strong>0</strong> to <strong>9</strong>.
- <strong>[_-]</strong> - string can contain <strong>underscore</strong> or <strong>hyphen</strong>.


<br>

### <strong>Character Classes</strong>

Character classes defines a set of character, any of which can occur in an input string to fulfill match.

- <strong>.</strong> - matches any character except the newline character (\n).
- <strong>\d</strong> - matches any Arabic numerical digit. Equivalent to the bracket expression [0-9] <strong>٠١٢٣٤٥٦٧٨٩.</strong>.
- <strong>\w</strong> - matches any alphanumeric character from the basic Latin alphabet, including the underscore.<strong>( _ )</strong>. Equivalent to the bracket expression [A-Za-z0-9_].
- <strong>\s</strong> - matches a single whitespace character, including tabs and line breaks.

Each of the last three character classes can be changed to perform an inverse match by capitalizing the letter character. For example, \D matches a non-digit character. 


<br>

### <strong>The OR Operator</strong>

Using OR operator <strong>( | )</strong> the expression [abc] could be written as <strong>( a | b | c ) </strong>.


<br>

### <strong>Flags</strong>

Flags is the one component that is an exception to the 'literal' rule.

Flags are placed at the end of a regex. After the second slash. They define additional functionality or limits for the regex. 

3 most common flags:
- <strong>g</strong> - Global search. Should be tested against all possible matches in string.
- <strong>i</strong> - Case-insensitive search. Case should be ignored while attempting a match in a string.
- <strong>m</strong> - Multi-line search. A multi-line input string should be trated as multiple lines.

<br>

### <strong>Character Escapes</strong>

Backlash <strong>( \ )</strong> in a regex escapes a character that otherwise would be interpreted literally.

<strong>( { )</strong> used to begin quantifier by adding backlas before <strong>( \ { )</strong> means regex should look for open curly braces instead.

<br>


### References

- [Coding bootcamp](https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)
- [Microsoft](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference)


<br> 

## Author

[Sara-Monintja](https://github.com/Sara-Monintja)

A barista turned full-stack developer obsessed with donut and obviously, coffee ☕️

Click on the donut for more [🍩](https://github.com/Sara-Monintja) 

