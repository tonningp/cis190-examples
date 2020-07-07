EXERCISES

Is each of the following an absolute pathname, a relative pathname, or a
simple filename?

a. milk_co

b. correspond/business/milk_co

c. /home/max

d. /home/max/literature/promo

eo.

f. letter.0210

List the commands you can use to perform these operations:
a. Make your home directory the working directory

b. Identify the working directory

If the working directory is /home/max with a subdirectory named
literature, give three sets of commands you can use to create a subdirectory
named classics under literature. Also give several sets of commands you can
use to remove the classics directory and its contents.

The df utility displays all mounted filesystems along with information about
each. Use the df utility with the —h (human-readable) option to answer the
following questions:

a. How many filesystems are mounted on the local system?
b. Which filesystem stores your home directory?

c. Assuming your answer to exercise 4a is two or more, attempt to create a
hard link to a file on another filesystem. What error message is displayed?
What happens when you attempt to create a symbolic link to the file
instead?

Suppose you have a file that is linked to a file owned by another user. How
can you ensure that changes to the file are no longer shared?

You should have read permission for the /etc/passwd file. To answer the fol-
lowing questions, use cat or less to display /etc/passwd. Look at the fields
of information in /etc/passwd for the users on the local system.

a. Which character is used to separate fields in /etc/passwd?
b. How many fields are used to describe each user?

c. How many users are on the local system?


EXERCISES 125

d. How many different login shells are in use on your system? (Hint: Look

at the last field.)

e. The second field of /etc/passwd stores user passwords in encoded form.
If the password field contains an x, your system uses shadow passwords
and stores the encoded passwords elsewhere. Does your system use
shadow passwords?

7. If/home/zach/draft and /home/max/letter are links to the same file and the
following sequence of events occurs, what will be the date in the opening of
the letter?

a. Max gives the command vim letter.
b. Zach gives the command vim draft.

c. Zach changes the date in the opening of the letter to January 31, writes
the file, and exits from vim.

d. Max changes the date to February 1, writes the file, and exits from vim.

8. Suppose a user belongs to a group that has all permissions on a file named
jobs_list, but the user, as the owner of the file, has no permissions. Describe
which operations, if any, the user/owner can perform on jobs_list. Which
command can the user/owner give that will grant the user/owner all permis-
sions on the file?

9. Does the root directory have any subdirectories you cannot search as an
ordinary user? Does the root directory have any subdirectories you cannot
read as a regular user? Explain.

10. Assume you are given the directory structure shown in Figure 4-2 on
page 85 and the following directory permissions:

d--x--x--- 3 zach pubs 512 2018-03-10 15:16 business
drwxr-xr-x 2 zach pubs 512 2018-03-10 15:16 business/milk_co

For each category of permissions—owner, group, and other—what happens
when you run each of the following commands? Assume the working direc-
tory is the parent of correspond and that the file cheese_co is readable by
everyone.

a. cd correspond/business/milk_co
b. ls -1 correspond/business

c. cat correspond/business/cheese_co


ADVANCED EXERCISES

What is an inode? What happens to the inode when you move a file within
a filesystem?

What does the .. entry in a directory point to? What does this entry point
to in the root (/) directory?

How can you create a file named -i? Which techniques do not work, and
why do they not work? How can you remove the file named -i?

Suppose the working directory contains a single file named andor. What
error message is displayed when you run the following command line?

$ mv andor and\/or

Under what circumstances is it possible to run the command without pro-
ducing an error?

The Is -i command displays a filename preceded by the inode number of the
file (page 115). Write a command to output inode/filename pairs for the
files in the working directory, sorted by inode number. (Hint: Use a
pipeline.)

Do you think the system administrator has access to a program that can
decode user passwords? Why or why not? (See exercise 6.)

Is it possible to distinguish a file from a hard link to a file? That is, given a
filename, can you tell whether it was created using an In command?
Explain.

Explain the error messages displayed in the following sequence of
commands:

$ 1s -1

drwxrwxr-x. 2 max pubs 1024 3-02 17:57 dirtmp
$ 1s dirtmp

$ rmdir dirtmp

rmdir: dirtmp: Directory not empty

$ rm dirtmp/*

rm: No match.


