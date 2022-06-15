# A Simple Shell built with C programming language

This simple shell - **grsh** - is a programm that provides an interface for users to get access to the kernel's services. It is a simple UNIX command intepreter. **grsh** is able to run default commands and someother commands have been built into it.

### Installation

First. Clone this repository in your machine.
```sh
$ git clone https://github.com/RaphaelAdewale/simple_shell.git
```
For best results, files should be compiled with
```sh
$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o grsh
```
### Usage

The grsh has two modes: **Interactive** in which the shell takes the commands from the standard input, executes them and gets ready to read another command-line.

As an example you can use the <b>ls</b> command for listing files in the current directory:

```sh
$ ls
_atoi.c AUTHORS built_ins.c _environ.c _error_handler.c main.h Makefile
```
The other mode is "Non-interactive". For this, the command should be passed thru a pipe
```sh
$ echo "/bin/ls" | ./grsh
_atoi.c AUTHORS built_ins.c _environ.c _error_handler.c main.h Makefile
```
### Included Built-Ins

Our shell has support for the following built-in commands:

| Command             | Definition                                                                                |
| ------------------- | ----------------------------------------------------------------------------------------- |
| exit [n]            | Exit the shell, with an optional exit status, n.                                          |
| env                 | Print the environment.                                                                    |
| setenv [var][value] | Set an environment variable and value. If the variable exists, the value will be updated. |
| unsetenv [var]      | Remove an environment variable.                                                           |
| cd [dir]            | Change the directory.                                                                     |
| help [built-in]     | Read documentation for a built-in.                                                        |
## Algorithm
![Flowchart](https://i.ibb.co/tpjpPw9/diagrama.png)

# Authors
* Gideon Adebowale [Email](mailto:gideonadebowale66@gmail.com)
* Raphael Adewale [Email](mailto:raphealadebomi@gmail.com)
