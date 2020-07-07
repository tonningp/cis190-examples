EXERCISES

# What does the shell ordinarily do while a command is executing? What should you do if you do not want to wait for a command to finish before
running another command?  

# Using sort as a filter, rewrite the following sequence of commands:

   $ sort list > temp
   $ lpr temp
   $ rm temp

# What is a PID number? Why are these numbers useful when you run processes in the background? Which utility displays the PID numbers of the commands
you are running?

# Assume the following files are in the working directory:

   $ ls
   intro notesb ref2 sectionl section3  section4b
   notesa ref1 ref3 section2 section4a sentrev

Give commands for each of the following, using wildcards to express filenames with as few characters as possible.

a. List all files that begin with section.
b. List the section1, section2, and section3 files only.
c. List the intro file only.
d. List the section1, section3, ref1, and ref3 files.

# Refer to Part VII or the info or man pages to determine which command will

   a. Display the number of lines in its standard input that contain the word a or A.
   b. Display only the names of the files in the working directory that contain the pattern $(.
   c. List the files in the working directory in reverse alphabetical order.
   d. Send a list of files in the working directory to the printer, sorted by size.

# Give a command to

a.  Redirect standard output from a sort command to a file named phone_list. Assume the input file is named numbers.

b. Translate all occurrences of the characters [ and { to the character (, and
all occurrences of the characters | and } to the character ), in the file
permdemos.c. (Hint: Refer to tr on page 1014.)

. Create a file named book that contains the contents of two other files:
part1 and part2.

7. The lpr and sort utilities accept input either from a file named on the command
line or from standard input.

a. Name two other utilities that function in a similar manner.

b. Name a utility that accepts its input only from standard input.

8. Give an example of a command that uses grep

a. With both input and output redirected.

b. With only input redirected.

c. With only output redirected.

d. Within a pipeline.

In which of the preceding cases is grep used as a filter?

9. Explain the following error message. Which filenames would a subsequent
Is command display?

$ 1s
abc abd abe abf abg abh
$ rm abc abs

rm: cannot remove

abc': No such file or directory

ADVANCED EXERCISES

10. When you use the redirect output symbol (>) on a command line, the shell
creates the output file immediately, before the command is executed.
Demonstrate that this is true.

 

 

ADVANCED EXERCISES 161

 

11.

12.

13.

14.

1S.

16.

In experimenting with variables, Max accidentally deletes his PATH variable.
He decides he does not need the PATH variable. Discuss some of the problems
he could soon encounter and explain the reasons for these problems. How
could he easily return PATH to its original value?

Assume permissions on a file allow you to write to the file but not to delete it.
a. Give a command to empty the file without invoking an editor.

b. Explain how you might have permission to modify a file that you cannot
delete.

If you accidentally create a filename that contains a nonprinting character,
such as a CONTROL character, how can you remove the file?

Why does the noclobber variable ot protect you from overwriting an
existing file with cp or mv?

Why do command names and filenames usually not have embedded spaces?
How would you create a filename containing a SPACE? How would you
remove it? (This is a thought exercise, not recommended practice. If you
want to experiment, create a file and work in a directory that contains only
your experimental file.)

Create a file named answer and give the following command:
$ > answers.0102 < answer cat

Explain what the command does and why. What is a more conventional
way of expressing this command?

