Given a string, return the middle character of the string.
If the string's length is odd, return the middle character. 
If the string's length is even, return the middle 2 characters.

# Examples

getMiddle("test") should return "es"
getMiddle("testing") should return "t"
getMiddle("middle") should return "dd"
getMiddle("A") should return "A"

# Input

A string of length 0 < str < 1000. 

# Output

The middle character(s) of the string, represented as another string.


# Task 2

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

# Specification

Create a solution that returns the sum of all numbers that are multiples of 3 or 5, and are smaller than a given number. 

# Examples

sum35(10) should return 23
sum35(200) should return 9168

# Input

An integer specifying the exclusive upper bound.

# Output

An integer containing the sum.



# Task 3
Markdown is a formatting syntax used by many documents (these instructions, for example!)
 because of its plain-text simplicity and its ability to be translated directly into HTML.

# Specification

Write a simple markdown parser function that will take in a single line of markdown 
and translate it into the appropriate HTML. To keep it simple, support only one feature of markdown in atx syntax: headers.
Headers are designated by 1-6 hash characters followed by a space, followed by text. The number of hashes determines the header level of the HTML output.

Header content should only come after the initial hashtag(s) plus a space character.
Invalid headers should just be returned as the markdown that was received, no translation necessary.
Spaces before the hashes and after the header should be kept in the output, but between the hashes and the text only one space is allowed.

# Examples

"# Header" should return "<h1>Header</h1>"
"## Header" should return "<h2>Header</h2>"
"###### Header" should return "<h6>Header</h6>"
"####### Header" should return "####### Header" (too many hashes)
"###  Header" should return "###  Header" (too many spaces between)
"Header" should return "Header" (no hashes)

# Input
A string that contains markdown text.

# Output
A string that contains html formatted text, if the input is valid markdown. Otherwise it just returns the input
