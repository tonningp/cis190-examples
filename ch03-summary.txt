CHAPTER SUMMARY

The utilities introduced in this chapter are a small but powerful subset of the many
utilities available on a typical system. Because you will use them frequently and
because they are integral to the following chapters, it is important that you become
comfortable using them.

The utilities listed in the following table  manipulate, display, compare, and print files.

Utility Functions (File utilities)

Utility  Function
   cp    Copies one or more files (page 53)
   diff  Displays the differences between two files (page 59)
   file  Displays information about the contents of a file (page 60)
   grep  Searches file(s) for a string (page 56)
   head  Displays the lines at the beginning of a file (page 57)
   lpq   Displays a list of jobs in the print queue (page 56)
   lpr   Places file(s) in the print queue (page 55)
   lprm  Removes a job from the print queue (page 56)
   mv    Renames a file or moves file(s) to another directory (page 54)
   sort  Puts a file in order by lines (page 58)
   tail  Displays the lines at the end of a file (page 57)
   uniq  Displays the contents of a file, skipping adjacent duplicate lines (page 58)

To reduce the amount of disk space a file occupies, you can compress it using
the bzip2 utility. Compression works especially well on files that contain pat-
terns, as do most text files, but reduces the size of almost all files. The inverse
of bzip2—bunzip2—restores a file to its original, decompressed form. Table 3-3
lists utilities that compress and decompress files. The bzip2 utility is the most efficient of these.

(De)compression utilities

Utility  Function
bunzip2  Returns a file compressed with bzip2 to its original size and format (page 65)
bzcat    Displays a file compressed with bzip2 (page 65)
bzip2    Compresses a file (page 64)
compress Compresses a file (not as well as bzip2 or gzip; page 66)
gunzip   Returns a file compressed with gzip or compress to its original size and format (page 66)
gzip     Compresses a file (not as well as bzip2; page 66)
unzip    Unpacks zip archives, which are compatible with Windows PKZIP
zcat     Displays a file compressed with gzip (page 66)
zip      Constructs zip archives, which are compatible with Windows PKZIP


An archive is a file, frequently compressed, that contains a group of files. The tar
utility (Table 3-4) packs and unpacks archives. The filename extensions .tar.bz2,
.tar.gz, and .tgz identify compressed tar archive files and are often seen on software
packages obtained over the Internet.

Archive utility
Utility  Function
tar      Creates or extracts files from an archive file (page 66)

The utilities listed in Table 3-5 determine the location of a utility on the local system.

For example, they can display the pathname of a utility or a list of C++ compilers
available on the local system.

Location utilities

Utility        Function
locate/mlocate Searches for files on the local system (page 70)
whereis        Displays the full pathnames of a utility, source code, or man page (page 69)
which          Displays the full pathname of a command you can run (page 69)

Table 3-6 lists utilities that display information about the local system and other users.
You can easily learn a user’s full name, login status, login shell, and other information
maintained by the system.

User and system information utilities

Utility  Function

finger   Displays detailed information about users, including their full names (page 72)
free     Displays memory usage information (page 74)
hostname Displays the name of the local system (page 53)
uptime   Displays system load and duration information (page 73)
w        Displays detailed information about users who are logged in on the local system (page 73)
who      Displays information about users who are logged in on the local system (page 71)

The utilities shown in Table 3-7 can help you stay in touch with other users on the local network.

User communication utilities

Utility  Function
mesg     Permits or denies messages sent by write (page 76)
write    Sends a message to another user who is logged in (page 75)

Table 3-8 lists miscellaneous utilities.

Miscellaneous utilities
Utility  Function
date     Displays the current date and time (page 62)
echo     Copies its arguments (page 1083) to the screen (page 61)
