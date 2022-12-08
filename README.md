# Challenge-17-Regex-Tutorial


## Introductory paragraph 
This is a tutorial which will be focussing on a specific regular expression or regex, explaining how the expression functions. A regex, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. 

## Summary
The regex that will be discussed in this tutorial will be 
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
This regex is used to verify that the string has the correct URL format and can also be used to extract the URL from a string. 


## Table of Contents

1. Anchors
2. Quantifiers
3. Grouping Constructs
4. Bracket Expressions
5. Character Classes
6. The OR Operator
7. Flags
8. Character Escapes


# Regex Components

## Anchors

The ^ and $ characters in this URL regex are known as the anchors. Anchors do not match a specific character, they match the positions before and after the characters, showing where the text begins and ends. The ^ character matches the beginning of the string or line, whereas the $ character matches the end of the string or line.  

## Quantifiers

A quantifier is used to determine how many times a specific character or a group of characters need to be present in order to have a match. A quantifier can be either greedy, meaning that it will be repeated as many times as possible or lazy meaning that it will repeat as few times as possible. 
The quanitifiers that are present in this URL are ?, +, * and { , } which are all greedy quantifiers. 
            1. The ? quantifier matches the preceding character one or zero times, making this character optional.
            2. The + quantifier matches the preceding element one or more times.
            3. The * quantifier matches the preceding element zero or more times

## Grouping Constructs

Group constructs bind expressions together to evaluate specific information in a specific order. This is done by enclosing part of the regex expresssion in parenthesis, which determines the order of processing. The first group in the URL regex is (https?:\/\/), this means that this match has to be true before the next part of the regex is processed. 

## Bracket Expressions

These are a list of characters which are enclosed in square brackets and used to match single characters or a range of characters in the expression. In the URL regex there two bracket expressions; [\da-z\.-], [a-z\.] and [\/\w \.-]. The expression [\da-z\.-], matches any lowercase a-z letter, and it can contain a hyphen and a period.

## Character Classes

Character classes can be used to instruct the engine to match only one out of the several characters. The notation \d is used to match any single digit, in this regex it will match any single character from a-z. 

## The OR Operator
The OR operator is also known as alternation, and is used when you want to choose between different characters. This is done by using the special character (vertical line) |. In the URL regex there is no OR operation, however an example is gra|ey which means gra or ey.

## Flags

A flag is used to change the default, changing the behavior of an expression. There are 6 flags which can be used and each have a different outcome. The flag i (insensitive) makes the search not distinguish between lower and upper cases such as Z and z. The flag g (global) makes the search look for many occurances, without it only the first match would be returned. The y (sticky) flag allows the match to search for a match at lastIndex exactly. 

## Character Escapes
Character escaping is when a special character is used as a regular one. This is done when a backslash is put in front of it. An example of a special charcter is a colon (:), this character is used to search in the contents of fields. To search for this character and give it its literal character meaning, you must escape it by adding the backslash (\:). In the URL regex that wer are looking at there are a few examples of character escapes one of them being (\.). Here the dot is usually a special character which matches any single character, however in this regex its being used as a regular character/

## References
https://www.oreilly.com/library/view/powershell-automating-administrative/9781787123755/ch21s02.html
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions
https://javascript.info/regexp-alternation#:~:text=Alternation%20is%20the%20term%20in,%2C%20PHP%2C%20Java%20or%20JavaScript.
https://www.w3schools.com/js/js_regexp.asp


## Author
Amal Hirsi
Email: ahirsi@hotmail.co.uk
Github: https://github.com/AmalHirsi