## Lab Report 2
# Code Change 1
The first change I made to the markdown file addresses the potential issue of non-url strings being printed by the file. This output is triggered by placing text inside parentheses after brackets that is not formatted correctly as a link `[sometext] (sometext)` instead of `[link](link)`.

![CodeChange1](CodeChange1.png)
This code was changed from the original Markdown file to remedy a bug when the following test-file was run:

[testfile1](https://github.com/jackmontoro/markdown-parse/commit/1ed204abaa4bb2bdf70c28d9edb75dfdb0023b65#diff-d902b3a6dba925548b7ea18ffb80dd0c28f1bc45f1d738a5da414273711a4409)

The program outputs `[cause an error, https://something.com, some-page.html]`.

After I fixed the code, the ouput was `[https://something.com, some-page.html]`.

# Code Change 2

# Code Change 3

# Code Change 4
