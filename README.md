# <a href="url"><img src="https://cdn3.iconfinder.com/data/icons/egg/500/Egg_food_cracked_whipped-512.png" align="middle" width="100" height="100"></a> simple_shell
simple_shell is a command line interpreter, or shell, in the tradition of the first Unix shell written by Ken Thompson in 1971. This shell is intentionally minimalistic, yet includes the basic functionality of a traditional Unix-like command line user interface. 
Standard functions and system calls employed in simple_shell include:
`access, execve, exit, fork, free, fstat, getline, malloc, perror, signal, stat, wait, write.`
* [AUTHORS](AUTHORS) - List of contributors to this repository
* [man_1_simple_shell](man_1_simple_shell) - Manual page for the simple_shell
* [shell.h](shell.h) - program header file
* [builtins.c](builtins.c) - major builtin functions
* `check_for_builtins` - checks to see if the user's command matches a builtin
* `new_exit` - exits the shell with the option of a specified status
* `_env` - prints the shell's environment variables to the standard output
* `new_setenv` - initializes a new environment variable, or modifies an existing one
* `new_unsetenv` - removes an environment variable
* [builtins2.c](builtins2.c) - helper functions for the builtins
* `add_key` - creates a new environment variable
* `find_key` - finds an environment variable in the environment array
* `add_value` - creates a new environment variable string
* `_atoi` - converts a string into a non-negative integer
* [environment.c](environment.c) - functions related to the environment
* `make_env` - creates the shell's environment from the parent process
* `free_env` - frees the shell's environment
* [errors.c](errors.c) - functions related to printing errors
* `print_error` - prints an error message to the standard error
* `_puts2` - prints a string to the standard error
* `_uitoa` - converts an unsigned integer to a string
* [memory_allocation.c](memory_allocation.c) - memory allocation functions
* `_realloc` - a custom realloc function for arrays of pointers
* [new_strtok.c](new_strtok.c) - custom strtok and helper functions
* `check_match` - checks if a character matches any in a string
* `new_strtok` - a custom strtok for the shell
* [path.c](path.c) - functions related to executing commands
* `path_execute` - executes a command in the PATH
* `find_path` - finds the PATH environment variable
* `check_for_path` - checks if the command is in the PATH
* `execute_cwd` - executes a command with an absolute path
* `check_for_dir` - checks if the command contains an absolute path
* [simple_shell.c](simple_shell.c) - essential functions to the shell
* `main` - the main function of the program
* `sig_handler` - handles SIGINT
* [strfunc.c](strfunc.c) - functions related to string manipulation
* `_puts` - writes a string to standart output
* `_strdup` - duplicates a string
* `_strcmpr` - compares two strings
* `_strcat` - concatenates two strings with a `/` in the middle
* `_strlen` - calculates the length of a string
* [tokenize.c](tokenize.c) - tokenizing function
* `tokenize` - creates an array of tokens from a buffer with a specified delimiter
## Authors
lola-source | [GitHub](https://github.com/lola-source)
Sayed Omari | [GitHub](https://github.com/omarisayed)

