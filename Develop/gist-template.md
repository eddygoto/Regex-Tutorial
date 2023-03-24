# Regex Tutorial: Matching an Email!

## Summary

In this tutorial, you will learn how to use regular expressions (regex) to match emails. The expression used for this purpose is /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. This can be helpful when validating emails using technologies such as Node (Inqurier) or MongoDB. The tutorial will cover the different components of a regex and demonstrate how they can be applied to match an email.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

Anchors are a way to indicate the start and end of the string being matched. In the regex for an email, "^" will indicate the beginning, and "$" will indicate the end. These anchors are essential because they ensure that the string is matched in its entirety; not just a substring that happens to contain a valid email address.

### Quantifiers

Quantifiers are used to specify how many times a particular pattern should be matched. In this specific regex expression, the "+" is used to connect the user's email name, their service, and .com. Another quantifier this regex uses is "{2,6}," which specifies a match range between 2 and 6 characters.

### Character Classes

A character class is a set of characters that can be matched by a single element of the regular expression. The "\d" characters class matches any digit character between 0 and 9. This can be useful for matching parts of an email address that include numbers, such as a user's email name.

### Grouping and Capturing

Capturing groups are used in regular expression to capture specific parts of a match for later use. In this regex, there are three capturing groups that match: the user email name, their service, and .com. These groups are indicated by the parentheses surrounding each pattern.

### Bracket Expressions

Bracket expressions define sets of characters that can be matched by a single element of the regex. This includes "[a-z0-9_\.-]," which matches any letter a-z, any number 0-9, and the special characters "_", "-", ".". "[\da-z\.-]," matches a single digit from 0-9, any character a-z, and the characters "." and "-".; "[a-z\.]" matches any character a-z and the character ".".

### Greedy and Lazy Match

"Greedy" matching means that a quantifier will try to match as much as possible, only backtracking if necessary to find a valid match. This is the default behavior in most regular expressions, and can sometimes result in unexpected matches. Lazy matching, on the other hand, tries to match as little as possible, and is indicated by the use of the "?" quantifier. Since this expression includes the "+" Quantifier, it will match as many times as possible giving back as needed.

## Author

You can view all my projects at https://github.com/eddygoto
