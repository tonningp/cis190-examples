CHAPTER SUMMARY

As with many operating systems, your access to a Linux system is authorized when
you log in. You enter your username in response to the login: prompt, followed by a
password. You can use passwd to change your password while you are logged in.

Choose a password that is difficult to guess and that conforms to the criteria imposed
by the system administrator.

The system administrator is responsible for maintaining the system. On a single-user
system, you are the system administrator. On a small, multiuser system, you or
another user will act as the system administrator, or this job might be shared. On a
large, multiuser system or network of systems, there is frequently a full-time system
administrator. When extra privileges are required to perform certain system tasks, the
system administrator gains root privileges by logging in as root or by running su or
sudo. On a multiuser system, several trusted users might be allowed to gain root
privileges.

Do not work with root privileges as a matter of course. When you have to do some-
thing that requires root privileges, work with root privileges for only as long as you
need to; revert to working as yourself as soon as possible.

The man utility provides online documentation on system utilities. This utility is helpful
both to new Linux users and to experienced users who must often delve into the system
documentation for information on the fine points of a utility’s behavior. The apropos
utility can help you search for utilities. The info utility helps the beginner and the expert
alike. It includes documentation on many Linux utilities. Some utilities, when called
with the —-help option, provide brief documentation on themselves.
