Shell Project
This project is a simple UNIX command-line interpreter, also known as a shell. It is capable of reading commands from standard input, parsing them, and executing them.

0x16. C - Simple Shell

 
AUTHORS file lists the contributors to the project.

README.md file you are currently reading is a brief overview of the project.

shell.h: a header file that includes all the necessary libraries, function prototypes, and global variables.

main.c: the main file that contains the loop for getting the user input, parsing the input, and executing the command.

prompt.c: a file that handles the prompt display for the shell.

execute.c: a file that contains the functions for executing the non-built-in commands.

builtins funcs: These are the source code files that contains functions related to the implementations of the built-in commands (cd, exit, env, setenv, unsetenv and help).

path funcs: These are the source code files that contains functions related to working with the system's PATH environment variable, such as finding a command in the PATH, getting the current PATH, and setting or modifying the PATH.

utils.c: a file that contains utility functions for the shell, such as string manipulation functions and functions for printing error messages.

error.c: This file contains the implementation of functions for handling errors.


Usage
To use the simple shell, compile the files using gcc -Wall -Werror -Wextra -pedantic *.c -o hsh. Then, run the shell using ./hsh.

gcc -Wall -Werror -Wextra -pedantic *.c -o$ ./hsh

($) ls

hsh main.c shell.c shell.h

$ exit
$
also in non-interactive mode:

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


AUTHORS
This program was written by Mariacelin Oshiomah <mariacelinoh@gmail.com>
