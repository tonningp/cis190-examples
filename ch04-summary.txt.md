CHAPTER SUMMARY

Linux has a hierarchical, or treelike, file structure that makes it possible to organize
files so you can find them quickly and easily. The file structure contains directory files
and ordinary files. Directories contain other files, including other directories; ordi-
nary files generally contain text, programs, or images. The ancestor of all files is the
root directory and is represented by / standing alone or at the left end of a pathname.

Most Linux filesystems support 255-character filenames. Nonetheless, it is a good
idea to keep filenames simple and intuitive. Filename extensions can help make file-
names more meaningful.

When you are logged in, you are always associated with a working directory. Your
home directory is the working directory from the time you log in until you use cd to
change directories.

An absolute pathname starts with the root directory and contains all the filenames
that trace a path to a given file. The pathname starts with a slash, representing the
root directory, and contains additional slashes following each of the directories in the
path, except for the last directory in the case of a path that points to a directory file.

A relative pathname is similar to an absolute pathname but traces the path starting
from the working directory. A simple filename is the last element of a pathname and
is a form of a relative pathname; it represents a file in the working directory.

A Linux filesystem contains many important directories, including /usr/bin, which
stores most of the Linux utilities, and /dev, which stores device files, many of which

 

 

CHAPTER SUMMARY 123

 

represent physical pieces of hardware. An important standard Linux file is
/etc/passwd; it contains information about users, such as a user’s ID and full name.

Among the attributes associated with each file are access permissions. They deter-
mine who can access the file and how the file may be accessed. Three groups of users
can potentially access the file: the owner, the members of a group, and all other users.
An ordinary file can be accessed in three ways: read, write, and execute. The Is utility
with the -I option displays these permissions. For directories, execute access is rede-
fined to mean that the directory can be searched.

The owner of a file or a user working with root privileges can use the chmod utility
to change the access permissions of a file. This utility specifies read, write, and exe-
cute permissions for the file’s owner, the group, and all other users on the system.

ACLs (Access Control Lists) provide finer-grained control over which users can
access specific directories and files than do traditional permissions. Using ACLs you
can specify the ways in which each of several users can access a directory or file. Few
utilities preserve ACLs when working with files.

An ordinary file stores user data, such as textual information, programs, or images.
A directory is a standard-format disk file that stores information, including names,
about ordinary files and other directory files. An inode is a data structure, stored on
disk, that defines a file’s existence and is identified by an inode number. A directory
relates each of the filenames it stores to an inode.

A link is a pointer to a file. You can have several links to a file so you can share the
file with other users or have the file appear in more than one directory. Because only
one copy of a file with multiple links exists, changing the file through any one link
causes the changes to appear in all the links. Hard links cannot link directories or
span filesystems, whereas symbolic links can.

Table 4-3 summarizes the utilities introduced in this chapter.

Utilities introduced in Chapter 4

Utility Function

cd Associates you with another working directory (page 94)
chmod Changes access permissions on a file (page 102)
getfacl Displays a file’s ACL (page 108)

In Makes a link to an existing file (page 113)

mkdir Creates a directory (page 93)

pwd Displays the pathname of the working directory (page 89)
rmdir Deletes a directory (page 96)

setfacl Modifies a file’s ACL (page 108)
