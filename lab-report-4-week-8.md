# Lab Report 4 - Week 8

## Markdown-parse repositories being reviewed

[My markdown-parse](https://github.com/ThisPorker/good-markdown-parser)

[Other group markdown-parse](https://github.com/UDXS/markdown-parser)


## Expected Output via CommonMark

### Snippet 1
![Snippet1](images/LR4/cmmrk1.png)
Expected output is `"google.com", "google.com", "ucsd.edu"`
### Snippet 2
![Snippet2](images/LR4/cmmrk2.png)
Expected Output is `"a.com", "a.com(())", "example.com"`
### Snippet 3
![Snippet3](images/LR4/cmmrk3.png)
Expected Output: `"https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule"`


## Test Code

![TestCode](images/LR4/TestCode2.png)


## My Implementation Result

![OurOutput](images/LR4/OurOutput.png)


## Their Implementation Result

![TheirOutput](images/LR4/TheirOutput.png)


## Question 1

Snippet 1 would probably require more than 10 lines of code to ammend. You would need to loop through each link and every character of each link input. Then check if it is an allowed character or symbol and ignore them if not.


## Question 2
Snippet 2 would require more than 10 lines of code. There are nested parenthesis which would be hard to determine which ones are actually being used and which should be ignored. There are a multiple issues with this snippet that can be as simple as ignoring backslashes before certain synax.


## Question 3
This snippet could probably be resolved with code that ignores newlines, in between brackets, and parenthesis. We might be able to keep track of the brackets or parenthesis, but any text inside of the brackets might require more code to keep it from showing up in the output. 
