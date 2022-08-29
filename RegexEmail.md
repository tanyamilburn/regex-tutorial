# Regex Tutorial: Matching an Email

This regular expression will allow you to see if a string is in email format. This is useful for when a user is required to include  a valid email as part of a signup process. 

## Summary
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This regex should match almost any email that is used. 
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
The ^ symbol is the beginning anchor. `{^[a-z0-9_\.-]}`+ --> This will match any email name that includes letters A-Z, numbers 0-9, periods, underscores, or hyphens. 


The $ symbol is the end anchor.  `{[a-z\.]{2,6}}`--> This will match any end of an email that includes letters A-Z or a period.

### Quantifiers
The quantifier `{{2,6}}` signifies a match with anywhere between 2-6 caharacters. 
### OR Operator
This defines what characters can be included in each section.
.`{^[a-z0-9.-]}` --> This will match any email name that includes letters A-Z, numbers 0-9, periods, or hyphens. 

### Character Classes
The section `{[\da-z\.-]}` includes the class `{\d}`.  This matches any Arabic numeral digit. This is a shorter way of expressing [0-9].

### Grouping and Capturing
The "Matching an Email" regex has three parts within parentheses. Each part is a string that should be grouped together.
`{([a-z0-9_\.-]+)}`
`{([\da-z\.-]+)}`
`{([a-z\.]{2,6})}`

### Bracket Expressions
We put patterns or positive character groups inside square brackets ([])  to create bracket expresssiongs. We can input a range of characters that want to match.
`{([a-z0-9_\.-]+)}`
`{([\da-z\.-]+)}`
These expressions are matching any letters a-z, numbers, and certain special characters. 

## Author
This was created by Tanya Milburn, a lowly bootcamp student. 
Check out more on my github!
[github.com/tanyamilburn](#www.github.com/tanyamilburn)
