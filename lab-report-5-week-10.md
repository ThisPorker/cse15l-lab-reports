# Lab Report 5 - Week 10
I used the command `diff` on the `test-results` file for `good-markdown-parse` (our group) and `markdown-parser` (Lab 9).  

`diff good-markdown-parser/markdown-parse/results.txt markdown-parser/results.txt > more-results.txt`

This sent the result of `diff` to a text file.

## Links to the test files

[Testfile519](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/519.md)
[Testfile543](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/543.md)

## Testing 519
Looking at the this test file, `uri3` should be the output, but it is not for either implementation.

![cmark519](images/LR5/cmark519.png)
 
Here is my Lab 9 test:
![Lab9Test519](images/LR5/Test519.png)

Here is my implemented test:
![impTest519](images/LR5/impTest519.png)

Results:
![Test519Result](images/LR5/Test519Result.PNG)

Issue: 

I believe the code below is not taking the results we want because the first set of parentheses are inside brackets and it is trying to use that instead of the result we are looking for. I believe the code block below would require some changing in how the program reads brackets and parentheses.

![bug519](images/LR5/Fix519.png)

## Testing 543
Analyzing this test file a blank result should be the output, but again my implementation and the given `markdown-parser` fails.

![cmark543](images/LR5/cmark543.png)

Here is my Lab 9 test:
![Lab9Test543](images/LR5/Test543.png)

Here is my implemented test:
![impTest543](images/LR5/impTest543.png)

Results:
![Test543Result](images/LR5/Test543Results.PNG)

Issue:

The problem here is with the variable types that are being passed. So the code block below would need changing along with whatever a change in variable type would cause. This might cascade into other issues, but I am not completely sure how to fix this issue.

![bug543](images/LR5/Fix543.png)