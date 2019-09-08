# Linux-cheat-sheet

> Click :star:if you like the project. Pull Request are highly appreciated. Follow me [@SudheerJonna](https://twitter.com/SudheerJonna) for technical updates.

### Table of Contents

* [**User information**](#user-information)
* [**File and directory commands**](#file-and-directory-commands)
* [**File permissions**](#file-permissions)
* [**Networking**](#networking)
* [**Installing packages**](#installing-packages)
* [**Disk usage**](#disk-usage)
* [**System and Hardware information**](#system-and-hardware-information)
* [**Search Files**](#search-files)
* [**SSH**](#ssh)
* [**Vi/Vim-commands**](#vi/vim-commands)


### User Information

1. **who** It is used to get information about currently logged in user on to system
   ```bash
   $ who
   sudheer :0 2019-08-04 01:21 (:0)
   ```
   1. **whoami:** It display the system’s username
   ```bash
   $ whoami
   sudheer
   ```
   2. **id:** It display the user identification information
   ```bash
   $ id

   ```
### File and directory commands
1. **pwd** The pwd(Present Working Directory) command is used to print the name of the present/current working directory starting from the root.
   ```bash
   $ pwd
   /home/sj/Desktop/Linux
   ```
2. **mkdir** The mkdir command allows users to create directories or folders.
   ```bash
   $ mkdir ubuntu
   $ ls
   ubuntu
   ```
   The option '-p' is used to create multiple directories or parent directories at once.
   ```bash
   $ mkdir -p dir1/dir2/dir3
   $ cd dir1/dir2/dir3
   ~/Desktop/Linux/dir1/dir2/dir3$
   ```
