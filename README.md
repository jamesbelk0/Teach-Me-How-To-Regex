# Teach-Me-How-To-Regex: RegEx - Matching an Email

Taking a look at regular expressions or Regex! Togeather we will be looking at how to break down regex looking for a matching an email. The characteristics that make up this expression are used to match validations, finding values that match and possibly replace them if needed! 

## Link to Gist File
- <https://gist.github.com/jamesbelk0/675d53938a619e78d31655651ea59803>
## Summary

In this tutorial we will be looking at the regular expression to find an email address. The regex we are looking at is the following: "/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/"

Below we will breakdown the concepts that make up the previous expression.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Author](#author)

## Regex Components

### Anchors
In our example the regex expression ends with the $. What this dictates is that the expression is finished and valid as long as it matches the previous quantifier. 

### Quantifiers
Quantifers indicate what characters will match. Throughout our exa,ple we have the + and the {2,6}. What this does is put a validation on our expression. 
- The + allows a match of one or more of the characters. In our example it will allow for single useage or duplicates of [a-z0-9_\.-]
- The {2,6} requires at least two characters with a max character count of 6 characters. 

### Grouping and Capturing
In the example above we have the following grouping: ([\da-z\.-]+)
This allows the user to capture any combination that can be contribed from the components inside. In this case we are seeing the following when broken down:
- \ = escapes a special character 
- d = any digit
- a-z = any lowercase letter 
- literal characters for a . or - 
- A + allows a match of one or more of the previous characters
This gives the user the power to input a wide variety of characters. 
### Bracket Expressions
In the example above, there are several bracket expressions or "[]". This is used when we have a range of characters that are to be used and saves us from having ot make a new grouping each time we need a change of characters. 
- For example [a-z0-9] is calling for all lowercase letters and any number 0-9.

## Author

Hello! My name is James Belk, a full-stack web developer who is always looking for something new to learn. When I am not at my computer I am at my gym helping others learn how to develop their bodies in a healthy way. To get a better understanding of my previous work please look at my repo that is attached below or if you have any questions please feel free to email me!

- <jamesbelk0@gmail.com>
- [GitHub](https://github.com/jamesbelk0)
