# Lab Report 4
---

## Tests for Our Implementation:
![Image](myTests.png)

## Tests for The Week 7 Implementation:
![Image](theirTests.png)

- Same tests as were used for our implementation

## Test Results for Our Implementation:
![Image](myFail.png)

- Each of the three tests failed

## Test Results for The Week 7 Implementation:
![Image](theirFail.png)

- Each of the three tests failed

## Discussion 

### Snippet 1:
- Since our implementation does not recognize 
backticks in a markdown file as a block of code, 
it still recognized url.com as a link, when it 
wasn't a valid link because the first bracket was 
betwen two backticks. Using an if statement to recognize backticks, you could move current index
to the index of the next backtick + 1, and then check if their was an open parentheses or bracket
in between those two backticks, and if so moving current index to the next open bracket. 

### Snippet 2:
- Our implementation failed the second test because of the way it made closeParen the first index of 
")" found in the while loop. To fix this, we could use a loop where closeParen is the indexOf(")", 
currentIndex) with current index updating to the most recently found ")" as long as it was less than 
the next index of "[".

### Snippet 3:
- To fix the output of snippet 3 would require markdown-parser to recognize line breaks where if 
they appear between an open and closed parentheses or bracket, that would invalidate the link and 
cause currentIndex to move to the next open bracket.
