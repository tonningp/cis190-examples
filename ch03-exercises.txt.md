EXERCISES

* Which commands can you use to determine who is logged in on a specific terminal?

* How can you keep other users from using write to communicate with you?
   Why would you want to?

* What happens when you give the following commands if the file named done already exists?

   $ cp to_do done
   $ mv to_do done

* How can you find out which utilities are available on your system for editing files? 
   Which utilities are available for editing on your system?

* How can you find the phone number for Ace Electronics in a file named phone that contains a list of names and phone numbers? 

* Which command can you use to display the entire file in alphabetical order? 

* How can you display the file without any adjacent duplicate lines? How can you display the file without any duplicate lines?

* What happens when you use diff to compare two binary files that are not identical? (You can use gzip to create the binary files.) 

* Explain why the diff output for binary files is different from the diff output for ASCII files.

* Create a .plan file in your home directory. Does finger display the contents of your .plan file?

 

* What is the result of giving the which utility the name of a command that resides in a directory that is not in your search path?

* Are any of the utilities discussed in this chapter located in more than one directory on the local system? If so, which ones?

* Experiment by calling the file utility with the names of files in /usr/bin. How many different types of files are there?

* Which command can you use to look at the first few lines of a file named status.report? 

* Which command can you use to look at the end of the file?

------------------------------------------------------------------------------------------------

ADVANCED EXERCISES

Re-create the colors.1 and colors.2 files used in Figure 3-8 on page 59. Test
your files by running diff -u on them. Does diff display the same results as
in the figure?

Try giving these two commands:

$ echo cat
$ cat echo

Explain the differences between the output of each command.

Repeat exercise 5 using the file phone.gz, a compressed version of the list
of names and phone numbers. Consider more than one approach to answer
each question and explain how you made your choices.

Find or create files that

a. gzip compresses by more than 80 percent.
b. gzip compresses by less than 10 percent.
c. Get larger when compressed with gzip.

d. Use Is -I to determine the sizes of the files in question. Can you charac-
terize the files in a, b, and c?

Older email programs were not able to handle binary files. Suppose you are
emailing a file that has been compressed with gzip, which produces a binary
file, and the recipient is using an old email program. Refer to the man page
on uuencode, which converts a binary file to ASCII. Learn about the utility
and how to use it.

a. Convert a compressed file to ASCII using uuencode. Is the encoded file
larger or smaller than the compressed file? Explain. (If uuencode is not on
the local system, you can install it using one of the tools described in
Appendix C; it is part of the sharutils package.)

b. Would it ever make sense to use uuencode on a file before compressing
it? Explain.

