Simple Shell Project in C

This project is about developing a simple Unix shell in C language, following the requirements listed below.

Requirements:

Allowed editors: vi, vim, emacs
All files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All files should end with a new line
A README.md file, at the root of the folder of the project is mandatory
The code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
The shell should not have any memory leaks
No more than 5 functions per file
All header files should be include guarded
Use system calls only when necessary
Write a README with the description of your project
Have an AUTHORS file at the root of your repository, listing all individuals having contributed content to the repository.
The repository should have only one project repository per group. If there are multiple repositories with the same name in both accounts, it will result in a 0% score. Add your partner as a collaborator.
Output:

The program should have the exact same output as the Unix shell (/bin/sh) and the exact same error output. The only difference is when an error is printed, the name of the program must be equivalent to argv[0].

List of allowed functions and system calls:

access, chdir, close, closedir, execve, exit, _exit, fflush, fork, free, getcwd, getline, getpid, isatty, kill, malloc, open, opendir, perror, read, readdir, signal, stat (__xstat), lstat (__lxstat), fstat (__fxstat), strtok, wait, waitpid, wait3, wait4, write.

Compilation:

The shell will be compiled using the following command:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh

Testing:

The shell should work in both interactive and non-interactive modes. The interactive mode should take commands from the user and execute them, while the non-interactive mode should execute the commands listed in a file. The shell should produce the same output and error messages as the Unix shell. Below are examples of the expected behavior:

Interactive mode:

$ ./hsh
($) /bin/ls
hsh main.c shell.c
($) exit
$

Non-interactive mode:

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

Authors:

This project is developed by [Chukwuma Emmanuella and Kelvin Karori].



