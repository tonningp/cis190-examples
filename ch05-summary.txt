CHAPTER SUMMARY

The shell is the Linux command interpreter. It scans the command line for proper syn-
tax, picking out the command name and arguments. The name of the command is
argument zero. The first argument is argument one, the second is argument two, and
so on. Many programs use options to modify the effects of a command. Most Linux
utilities identify an option by its leading one or two hyphens.

When you give it a command, the shell tries to find an executable program with the
same name as the command. When it does, the shell executes the program. When it
does not, the shell tells you it cannot find or execute the program. If the command is
a simple filename, the shell searches the directories listed in the PATH variable to
locate the command.

When it executes a command, the shell assigns one file or device to the command’s
standard input and another file to its standard output. By default, the shell causes a
command’s standard input to come from the keyboard and its standard output to go
to the screen. You can instruct the shell to redirect a command’s standard input from
or standard output to any file or device. You can also connect standard output of one
command to standard input of another command to form a pipeline. A filter is a com-
mand that reads its standard input from standard output of one command and writes
its standard output to standard input of another command.

When a command runs in the foreground, the shell waits for the command to finish
before it displays a prompt and allows you to continue. When you put an ampersand
(&) at the end of a command line, the shell executes the command in the background
and displays another prompt immediately. Run slow commands in the background
when you want to enter other commands at the shell prompt. The jobs builtin dis-
plays a list of suspended jobs and jobs running in the background and includes the
job number of each.

The shell interprets special characters on a command line to generate filenames. A
reference that uses special characters (wildcards) to abbreviate a list of one or more
filenames is called an ambiguous file reference. A question mark represents any single
character, and an asterisk represents zero or more characters. A single character
might also be represented by a character class: a list of characters within brackets.

A builtin is a utility that is built into a shell. Each shell has its own set of builtins.
When it runs a builtin, the shell does not fork a new process. Consequently builtins
run more quickly and can affect the environment of the current shell.

UTILITIES AND BUILTINS INTRODUCED IN THIS CHAPTER

Table 5-1 lists the utilities introduced in this chapter.

New utilities
Utility Function
tr Maps one string of characters to another (page 146)
tee Sends standard input to both a file and standard output (page 149)
bg Moves a process to the background (page 151)
fg Moves a process to the foreground (page 151)

jobs Displays a list of suspended jobs and jobs running in the background (page 152)

