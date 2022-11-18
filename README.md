# Challenge-17-Regex-Tutorial
Title  Challenge-17-Regex-Tutorial

Introductory paragraph 
This is a tutorial which will be focussing on a specific regular expression or regex, explaining how the expression functions. A regex, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. 

Summary
The regex that will be discussed in this tutorial will be 
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
This regex is used to verify that the string has the correct URL format and can also be used to extract the URL from a string. 


Table of Contents

Anchors
Quantifiers
Grouping Constructs
Bracket Expressions
Character Classes
The OR Operator
Flags
Character Escapes


Regex Components

Anchors
The ^ and $ characters in this URL regex are known as the anchors. Anchors do not match a specific character, they match the positions before and after the characters, showing where the text begins and ends. The ^ character matches the beginning of the string or line, whereas the $ character matches the end of the string or line.  

Quantifiers
A quantifier is used to determine how many times a specific character or a group of characters need to be present in order to have a match. A quantifier can be either greedy, meaning that it will be repeated as many times as possible or lazy meaning that it will repeat as few times as possible. 
The quanitifiers that are present in this URL are ?, +, * and { , } which are all greedy quantifiers. 
            1. The ? quantifier matches the preceding character one or zero times, making this character optional.
            2. The + quantifier matches the preceding element one or more times.
            3. The * quantifier matches the preceding element zero or more times

Grouping Constructs
Group constructs bind expressions together to evaluate specific information in a specific order. This is done by enclosing part of the regex expresssion in parenthesis, which determines the order of processing. The first group in the URL regex is (https?:\/\/), this means that this match has to be true before the next part of the regex is processed. 

Bracket Expressions

Character Classes

The OR Operator

Flags

Character Escapes

References
https://www.oreilly.com/library/view/powershell-automating-administrative/9781787123755/ch21s02.html
Author
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)