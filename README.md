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
2. **mkdir** The mkdir(make directory) command allows users to create directories or folders.
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
3. **rm**: The rm(remove) command is used to  remove objects such as files, directories, symbolic links etc from the file system.
   1. Remove file: The rm command is used to remove or delete a file
   ```bash
   rm file_name
   ```
   2. Remove file forcefully: The rm command with -f option is used for removal of file without prompting for confirmation.
   ```bash
   rm -f filename
   ```
   3. Remove directory: The rm command with -r option is used to remove the directory and its contents recursively.
   ```bash
   rm -r myDir
   ```
   4. Remove directory forcefully: The rm command with -rf option is used to forcefully remove directory recursively.
   ```bash
   rm -rf myDir
   ```
4. **touch**: The touch command is is used to create, change and modify timestamps of a file without any content.
   1. Create a new file: You can create a single file at a time using touch command. The file created is an empty file.
   ```bash
   touch file_name
   ```
   2. Create multiple files: You can create the multiple numbers of files at the same time.
   ```bash
   touch file1_name file2_name file3_name
   ```
   3. Change access time: The touch command with `a` option is used to change the access time of a file.
   ```bash
   touch -a file_name
   ```
   4. Change modification time: The touch command with `m` option is used to change the modified time.
   ```bash
   touch -m file_name
   ```
   5. Use timestamp of other file: The touch command with `r` option is used to get timestamp of another file.
   ```bash
   touch -r file2 file1
   ```
   In the above example, we get the timestamp of file1 for file2.
   6. Create file with Specific time: The touch command with 't' option is used to create a file with specified time.
   ```bash
   touch -t 1911010000 file_name
   ```
5. **cat**: The cat command is used to create single or multiple files, view contain of file, concatenate files and redirect output in terminal or files.