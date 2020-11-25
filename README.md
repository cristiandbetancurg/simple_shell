### 📝 Description

The following project is based on the legendary C programming language. This project is based on simulating a real Shell with limited functions, I have done it for Holberton School as part of my final project for the first term of study.

### 💾 For your installation and testing

You can clone my repository in your working directory or download it directly to your PC. I recommend that you compile with GCC 9.3 or higher and with the following flags: -Wall -Wextra -Werror -pedantic -Wno-format.

### 💻 Usage

Once you compile you can run it or start the program independently and in interactive mode or Non-Interactive Mode.

#### 🕹 Interactive Mode

In interactive mode, simply run the program and wait for the prompt to appear. From there, you can type commands freely, exiting with either the "exit" command or ctrl-D.

#### 🕹 Non-Interactive Mode

In non-interactive mode, echo your desired command and pipe it into the program like this:

```sh
echo "ls" | ./shell
```


#### ⌨ Included Built-Ins

Our shell has support for the following built-in commands:

| Command             | Definition                                                                                |
| ------------------- | ----------------------------------------------------------------------------------------- |
| exit [n]            | Exit the shell, with an optional exit status, n.                                          |
| env                 | Print the environment.                                                                    |
| setenv [var][value] | Set an environment variable and value. If the variable exists, the value will be updated. |
| unsetenv [var]      | Remove an environment variable.                                                           |
| cd [dir]            | Change the directory.                                                                     |
| help [built-in]     | Read documentation for a built-in.                                                        |


#### 📢 Outside Programs

Our shell can run outside programs by typing their absolute paths (/bin/ls) or the executable name (ls), IF their directory is included in the PATH.

### ✏ Examples

```sh
$ ls -l
total 8
drwxrwxr-x 1 vagrant vagrant Apr 2 13:23 directory_1
drwxrwxr-x 2 vagrant vagrant Apr 2 20:30 directory_2
```

```sh
$ /bin/pwd
/home/vagrant/shell
```

```sh
$ hello world
./hsh: 1: hello: not found
```

```sh
$ help env
env: env
	Print the environment.
```

### 📚 Included Files

- main.c - functions for calling the shell and initializing the shell struct
- shell.c - functions for running the basic shell logic
- shell_helpers.c - functions for helping the shell run
- split_string.c - functions for splitting string from the user
- string_helpers1.c - functions for manipulating strings
- string_helpers2.c - functions for manipulating strings
- built_ins.c - functions for built-ins
- built_in_helpers.c - functions for helping the built-in functions
- help.c - functions for the help built-in
- help2.c - functions for the help built-in
- cd.c - functions for the cd built-in
- cd2.c - functions for the cd built-in
- \_getenv.c - functions for getting elements from the environment
- env.c - functions for the env, setenv, and unsetenv built-ins
- llfuncs1.c - linked list functions
- llfuncs2.c - linked list functions
- expansions.c - functions for dealing with the $? and $\$ expansions
- check_path.c - functions for checking the path of an executable
- error_handler.c - functions for dealing with errors
- free.c - functions for freeing allocated memory
- holberton.h - header file

### 👨‍💻 Author

by [Cristian Betancur](https://twitter.com/cryptocoincanal) 
