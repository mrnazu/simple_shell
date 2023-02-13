# simple_shell

```By: Julien Barbier
Weight: 10
team: Samuel Amsalu, Chinedu Prince
Project must end by Feb 22
Checker will be released at Feb 21
```
## General

   -  Who designed and implemented the original Unix operating system
   -  Who wrote the first version of the UNIX shell
   -  Who invented the B programming language (the direct predecessor to the C programming language)
   -  Who is Ken Thompson
   -  How does a shell work
   -  What is a pid and a ppid
   -  How to manipulate the environment of the current process
   -  What is the difference between a function and a system call
   -  How to create processes
   -  What are the three prototypes of main
   -  How does the shell use the PATH to find the programs
   -  How to execute another program with the execve system call
   -  How to suspend the execution of a process until one of its children terminates
   -  What is EOF / “end-of-file”?

## Requirements

   -  Allowed editors: vi, vim, emacs
   -  All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
   -  All your files should end with a new line
   -  A README.md file, at the root of the folder of the project is mandatory
   -  Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
   -  Your shell should not have any memory leaks
   -  No more than 5 functions per file
   -  All your header files should be include guarded
   -  Use system calls only when you need to (why?)
   -  Write a README with the description of your project
   -  You should have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository. Format, see Docker

Your shell will be compiled this way:
```
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```
Your shell should work like this in interactive mode:
```
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```
But also in non-interactive mode:
```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```

