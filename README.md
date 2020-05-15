# Linux-cheat-sheet

> Click :star:if you like the project. Pull Request are highly appreciated. Follow me [@SudheerJonna](https://twitter.com/SudheerJonna) for technical updates.

### Table of Contents
-------------------------------------------------------------------
| No. | Topic |
|---- | ---------
|1  | [**User information**](#user-information) |
|2  | [**File and directory commands**](#file-and-directory-commands) |
|3  | [**File permissions**](#file-permissions) |
|4  | [**Networking**](#networking) |
|5  | [**Installing packages**](#installing-packages) |
|6  | [**Disk usage**](#disk-usage) |
|7  | [**System and Hardware information**](#system-and-hardware-information) |
|8  | [**Search Files**](#search-files) |
|9  | [**SSH**](#ssh)
|10 | [**Vi/Vim-commands**](#vi/vim-commands) |


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

   **[⬆ Back to Top](#table-of-contents)**

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
   1. View file contents: You can view contents of a single or more files by mentioning the filenames.
   ```bash
   cat file_name1 file_name2
   ```
   2.

   **[⬆ Back to Top](#table-of-contents)**

### File permissions

   **[⬆ Back to Top](#table-of-contents)**

### Networking

   **[⬆ Back to Top](#table-of-contents)**

### Installing packages

   **[⬆ Back to Top](#table-of-contents)**

### Disk usage

   **[⬆ Back to Top](#table-of-contents)**

### System and Hardware information

   **[⬆ Back to Top](#table-of-contents)**

### Search Files

   **[⬆ Back to Top](#table-of-contents)**

### SSH

   **[⬆ Back to Top](#table-of-contents)**

### Vi/Vim-commands

   Vi editor is the most popular text editor from the early days of Unix. Whereas Vim(Vi IMproved) is an improved version of vi editor to be used in CLI (command line interface) for mainly text editing tasks in many configuration files. Some of the other alternatives are Elvis, Nvi, Nano, Joe, and Vile.
   It has two main operation modes,

   1. **Command Mode:** It allows the entry of commands to manipulate text.
   2. **Entry mode(Or Insert mode):** It allows typed characters on the keyboard into the current file.

#### 1. Start with Vi Editor

   You can create a new file or open an existing file using `vi filename` command.
   ```cmd
    vi <filename_NEW> or <filename_EXISTING> // Create a new file or open an existing file

    Example:
    vi first.txt
   ```
   Let's see how do you create file, entre the content and leave the CLI by saving the changes.
   1. Create a new file named `first.txt`
   2. Press `i` to enter the insert mode
   3. Enter the text "Hello World!"
   4. Save the text and exit by pressing `:wq!` command
   5. Check the entered text

#### 2. Cursor movement
    These commands will be used in Command mode.

##### Move cursor
   You can use arrow keys(left, right, up and down) to move the cursor on the terminal. But you can also other keys for this behavior.
   ```cmd
    h        # Move left
    j        # Move down
    k        # Move up
    l        # Move right
   ```
##### Jump one word
   These commands used to jump one word at a time
   ```cmd
   w        # Jump forwards to the start of a word
   W        # Jump forwards to the start of a WORD
   e        # Jump forwards to the start of a word
   E        # Jump forwards to the start of a WORD
   b        # Jump backwords to the start of a word
   B        # Jump backwords to the start of a WORD
   ```

##### Move to start or end of a line
   These commands used to move starting or ending of a line.
   ```cmd
   ^        # Jump to the start of a current line
   $        # Jump to the end of a current line
   ```

   **[⬆ Back to Top](#table-of-contents)**