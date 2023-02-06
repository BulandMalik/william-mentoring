## Unix Commands

>cd DIR_NAME

>ls -l

>ls -a

>ls -las

### Pipes

Pipes used to pass output of one command as an input of another command

>Count the total # of words inb the `ls` command output <br/>
```ls | wc -w``` <br/>
```cat file1.txt file2.txt | wc -w```

### Redirection

Standard Input (stdin) = 0
Standard Output (stdout) = 1
Standard Error (stderr) = 2

>use ```<``` for input

>use ```>``` for output

>use ```2>``` for error

>use ```2>&1``` for error + output

>Create a file input.txt with the text user enters <br/>```cat < input.txt```

>Stores output in a file using ```>``` <br/>
```ls -las /usr/bin > output.txt```

>Redirecting errors to an error file (changing default stderr) `2>` <br/>
```ls -las /usr/DO_NOt_EXISTS 2> error.txt```

>Redirecting errors to an error or actual output to same file using `2>&1` <br/>
```ls -las /usr/DO_NOt_EXISTS > error_and_output.txt 2>&1```

### Grep
It stands for `Global regular expression print`.

It is used to search within folders & files as well as contents of the files.

It is case sensitive.

>Search text starts with `Mon` in file letter.txt <br/>
```grep Mon letter.txt```

>Search text that has `mon` in file letter.txt <br/>
```grep mon letter.txt```

>Search text starts with `Mon` in file letter.txt. `-i` ignore case sensitivity <br/>
```grep -i Mon letter.txt```

>Search text that exactly match word `Monday` in file letter.txt. `-w` does the exact match <br/>
```grep -w Monday letter.txt```

>Searches specific folder from ls command result. <br/>
```ls /bin | grep zip```

>You have a text file that contains addresses. You would like to search for addresses with the word “Ocean”, so you perform a grep search with no additional flags. In this case, which one of the following statements would be true?  
>>Yes that is true

<br/><hr/>

>The options you pass to a command are known as `Flags`

>To pass the output from one command as the input to another command, we use `Pipes`

<br/><hr/>

### Additional Resources

[Agile methodologies](https://www.planview.com/resources/guide/agile-methodologies-a-beginners-guide/)

[Installing git on mac and windows, detailed instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

[Bash Reference Manual](https://www.gnu.org/software/bash/manual/html_node/index.html#SEC_Contents)

[Bash Redirections](https://www.gnu.org/software/bash/manual/html_node/Redirections.html#Redirections)

[Bash Cheatsheet](https://devhints.io/bash)

[Grep Cheatsheet](https://devhints.io/grep)

[Grep Manual](https://man7.org/linux/man-pages/man1/grep.1.html)

[History and Timeline of Unix](https://unix.org/what_is_unix/history_timeline.html)

[History of Vim](https://en.wikipedia.org/wiki/Vim_(text_editor))

[How to work with relative and absolute paths](https://www.geeksforgeeks.org/absolute-relative-pathnames-unix/)

[Unix Commands Cheatsheet](https://cheatography.com/jluis/cheat-sheets/bash-and-unix-commands/)

[Vim Cheatsheet](https://vim.rtorr.com/)
