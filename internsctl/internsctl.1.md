% INTERNSCTL(1) internsctl 0.1.0
% Mohd Kashif Khan
% August 2021

# NAME
internsctl - get CPU, memory and file's info. Creates and lists users.

# SYNOPSIS
**internsctl** *COMMAND*\
**internsctl** *COMMAND* [*OPTION*] [*USERNAME*]\
**internsctl** *COMMAND* [*OPTION*]... *FILENAME*\
\

# DESCRIPTION
**internsctl** fetches the CPU info , memory usage and properties of a file. **internsctl** has to be run with certain commands. It also creates the user with provided username.
Running **internsctl** with proper options gets you the specific properties of a file.

# COMMANDS
The understood commands are :

**cpu getinfo**
: Displays all the information about the CPU of the server.

**memory getinfo**
: Displays the current RAM usage on the server.

**user create** *USERNAME*
: Creates the user with its home directory and ramdom password of 8 charcters of length.

**user list** [--sudo-only]
: Lists out all the regular users.
  With option, it lists out all the users with sudo privileges.

**file getinfo** *FILENAME*
: Displays the name, size, owner, permissions and the last modified date of a file.

The options associated with **file getinfo** [*OPTIONS*]... *FILENAME* are:
	
**-s**, **--size**
: Displays size of the file.
	
**-p**, **--permissions**
: Displays access permissions of the file.

**-o**, **--owner**
: Displays owner of the file.

**-m**, **--last-modified**
: Displays last modified time of the file.

# OPTIONS
**-h**, **--help**
: Displays a friendly help message.

**-V**, **--version**
: Displays the software version.

# EXIT VALUES
**0**
: Success

**1**
: Invalid option or command failed.

# COPYRIGHT
Copyright © 2021 Mohd Kashif Khan.This is free software: you are free to change and redistribute it.
