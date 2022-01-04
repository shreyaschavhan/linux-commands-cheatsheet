`Note: These are my notes for personal reference!`



## 𝐁𝐚𝐬𝐢𝐜

- `date` : displays the current time and date
```
┌──(shreyas㉿kali)-[~]
└─$ date
Tuesday 04 January 2022 03:39:43 PM IST
```                        

---

- `cal` : displays a calendar of the current month
```
┌──(shreyas㉿kali)-[~]
└─$ cal  
    January 2022      
Su Mo Tu We Th Fr Sa  
                   1  
 2  3  4  5  6  7  8  
 9 10 11 12 13 14 15  
16 17 18 19 20 21 22  
23 24 25 26 27 28 29  
30 31                 

```
---

- `df` : the current amount of free space on our disk drives
```
┌──(shreyas㉿kali)-[~]
└─$ df  
Filesystem     1K-blocks     Used Available Use% Mounted on
udev             1953436        0   1953436   0% /dev
tmpfs             399160     1168    397992   1% /run
/dev/sda1      130538556 11247868 112613492  10% /
tmpfs            1995784        0   1995784   0% /dev/shm
tmpfs               5120        0      5120   0% /run/lock
tmpfs             399156       68    399088   1% /run/user/1000
              
```
---
- `free` : display the amount of free memory
```
┌──(shreyas㉿kali)-[~]
└─$ free                      
               total        used        free      shared  buff/cache   available
Mem:         3991568      672232     2753624        8864      565712     3079888
Swap:         998396           0      998396
            
```
---

## 𝐍𝐚𝐯𝐢𝐠𝐚𝐭𝐢𝐨𝐧

- `pwd` : print working directory
```
┌──(shreyas㉿kali)-[~]
└─$ pwd                
/home/shreyas
                
```
---

- `cd` : change directory
```
┌──(shreyas㉿kali)-[~]
└─$ cd practise           
                                                                                       
┌──(shreyas㉿kali)-[~/practise]
└─$ pwd
/home/shreyas/practise
                                                                                       
┌──(shreyas㉿kali)-[~/practise]
└─$ ls 
hackthebox

```
---

- `cd` shortcuts

Shortcut | Result
---|---
cd | Changes the working directory to your home directory.
cd - | Changes the working directory to the previous working directory.
cd ~user_name | Changes the working directory to the home directory of user_name. For example, typing cd ~bob will change the directory to the home directory of user “bob.”

---

- `ls` : List directory contents
>   - `ls -l`: output in long format
>   - `ls -t`: the t option to sort the result by the file’s modification time.
>   - `ls -lt --reverse`: --reverse to reverse the order of the sort.
```
┌──(shreyas㉿kali)-[~]
└─$ ls
BugBounty  Documents  Music     practise  Templates
Desktop    Downloads  Pictures  Public    Videos
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ ls /usr      
bin  games  include  lib  lib32  lib64  libexec  libx32  local  sbin  share  src
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ ls practise /usr
practise:
hackthebox

/usr:
bin  games  include  lib  lib32  lib64  libexec  libx32  local  sbin  share  src
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ ls -l          
total 176
drwxr-xr-x  3 shreyas shreyas  4096 Jan  1 17:38 BugBounty
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Desktop
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Documents
drwxr-xr-x  3 shreyas shreyas  4096 Dec 29 15:32 Downloads
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Music
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Pictures
drwxr-xr-x  3 shreyas shreyas  4096 Dec 26 21:40 practise
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Public
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Templates
drwxr-xr-x  2 shreyas shreyas  4096 Dec 14 19:34 Videos

                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ ls -lt
total 40
drwxr-xr-x 3 shreyas shreyas 4096 Jan  1 17:38 BugBounty
drwxr-xr-x 3 shreyas shreyas 4096 Dec 29 15:32 Downloads
drwxr-xr-x 3 shreyas shreyas 4096 Dec 26 21:40 practise
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Desktop
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Documents
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Music
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Pictures
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Public
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Templates
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Videos

                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ ls -lt --reverse                                                               2 ⨯
total 40
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Videos
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Templates
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Public
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Pictures
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Music
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Documents
drwxr-xr-x 2 shreyas shreyas 4096 Dec 14 19:34 Desktop
drwxr-xr-x 3 shreyas shreyas 4096 Dec 26 21:40 practise
drwxr-xr-x 3 shreyas shreyas 4096 Dec 29 15:32 Downloads
drwxr-xr-x 3 shreyas shreyas 4096 Jan  1 17:38 BugBounty
                                                                                       
```
---

- `file filename` :  the file command will print a brief description of the file’s contents
```
┌──(shreyas㉿kali)-[~/practise/hackthebox]
└─$ file flag.txt             
flag.txt: ASCII text, with no line terminators
                                                                                       
┌──(shreyas㉿kali)-[~/practise/hackthebox]
└─$ file pack.ovpn 
pack.ovpn: ASCII text

```
---

- `less` : allows us to scroll forward and backward through a text file.
  - `Note: less is more. Means both commands are same` 
```
┌──(shreyas㉿kali)-[~/practise/hackthebox]
└─$ cat example | less
                                                                                       
┌──(shreyas㉿kali)-[~/practise/hackthebox]
└─$ less example
```

Command | Action
--- | ---
`PAGE UP` or `b` | Scroll back one page
`PAGE DOWN` or `space` | Scroll forward one page
`Up arrow` | Scroll up one line
`Down arrow` | Scroll down one line
`G` | Move to the end of the text file
`1G` or `g` | Move to the beginning of the text file
`/characters` | Search forward to the next occurrence of characters
`n` | Search for the next occurrence of the previous search
`h` | Display help screen
`q` | Quit less


---

## 𝐌𝐚𝐧𝐢𝐩𝐮𝐥𝐚𝐭𝐢𝐧𝐠 𝐟𝐢𝐥𝐞𝐬 𝐚𝐧𝐝 𝐝𝐢𝐫𝐞𝐜𝐭𝐨𝐫𝐢𝐞𝐬

- Wildcards:

Wildcards | Meaning
--- | ---
`*` | Matches any character
`?` | Matches any single character
`[characters]` | Matches any character that is a member of the set characters
`[!characters]` | Matches any character that is not a member of the set characters
`[:class:]]` | Matches any character that is member of the specified class

- List of most commonly used character classes

Character class | Meaning
--- | ---
`[:alnum:]` | Matches any alphanumeric character
`[:alpha:]` | Matches any alphabetic characters
`[:digit:]` | Matches any numerical
`[:lower:]` | Matches any lowercase letter
`[:upper:]` | Matches any uppercase


- Wildcard examples:

Pattern | Matches
--- | ---
`*` | All files
`g*` | Any file beginning with g
`b*.txt` | Any file beginning with b followed by any characters and ending with .txt
`Data???` | Any file beginning with Data followed by exactly three characters
`[abc]*` | 	Any file beginning with either an a, a b, or a c
`BACKUP.[0-9][0-9][0-9]` | Any file beginning with BACKUP. followed by exactly three numerals
`[[:upper:]]*` | Any file beginning with an uppercase letter
`[![:digit:]]*` | Any file not beginning with a numeral
`*[[:lower:]123]` | Any file ending with a lowercase letter or the numerals 1, 2, or 3

- `Wildcards can be used with any command that accepts filenames as arguments`

---

- `mkdir` - make directory
    - `mkdir dir` - single directory
    - `mkdir dir1 dir2 dir3` - multiple directories
    
    
```
┌──(shreyas㉿kali)-[~/practise]
└─$ mkdir commandline
                                                                                       
┌──(shreyas㉿kali)-[~/practise]
└─$ ls          
commandline  hackthebox

┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ mkdir dir1 dir2 dir3
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ ls
dir1  dir2  dir3

```
---

- `cp` - copy files and directories
    - `cp item1 item2` : copy single file item1 into item2
    - `cp item... directory` : copies multiple items (either files or directories) into a directory.

Option | Meaning
--- | ---
`-a`,`--archive` | Copy the files and directories and all of their attributes, including ownerships and permissions.
`-i`, `--interactive` | Before overwriting an existing file, prompt the user for confirmation. 
`-r`, `--recursive` | Recursively copy directories and their contents. This option (or the -a option) is required when copying directories.
`-u`, `--update` | When copying files from one directory to another, only copy files that either don’t exist or are newer than the existing corresponding files in the destination directory. This is useful when copying large numbers of files as it skips files that don’t need to be copied
`-v`, `--verbose` | Display informative messages as the copy is performed.

- `mv` is same as `cp`

---

- `rm file` : remove files and directories


Option | Meaning
--- | ---
`-i`, `--interactive` | Before deleting an existing file, prompt the user for confirmation.
`-r`, `--recursive` | Recursively delete directories. This means that if a directory being deleted has subdirectories, delete them too. To delete a directory, this option must be specified.
`-f`, `--force` | Ignore nonexistent files and do not prompt. This overrides the --interactive option.
`-v`, `--verbose` | Display informative messages as the deletion is performed.

---

- `ln` : create links
    - `ln file link` : create a hard link
    - `ln -s item link` : creates a symbolic link

---

## 𝐖𝐨𝐫𝐤𝐢𝐧𝐠 𝐰𝐢𝐭𝐡 𝐜𝐨𝐦𝐦𝐚𝐧𝐝𝐬

- `type`: is a shell builtin that displays the kind of command the shell will execute

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ type ls      
ls is an alias for ls --color=auto
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ type ssh
ssh is /usr/bin/ssh
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ type cd 
cd is a shell builtin
                          
```
---

- `which` : Display an Executable’s Location

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ which ls           
ls: aliased to ls --color=auto
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ which pwd
pwd: shell built-in command
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ which cd 
cd: shell built-in command
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ which gedit
/usr/bin/gedit
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ which firefox
/usr/bin/firefox
                       
```

---

- `man` : Display a Program’s Manual Page

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ man ls         
```

```
LS(1)                               User Commands                              LS(1)

NAME
       ls - list directory contents

SYNOPSIS
       ls [OPTION]... [FILE]...

DESCRIPTION
       List  information  about  the FILEs (the current directory by default).  Sort
       entries alphabetically if none of -cftuvSUX nor --sort is specified.

       Mandatory arguments to long options are mandatory for short options too.

       -a, --all
              do not ignore entries starting with .

       -A, --almost-all
              do not list implied . and ..

       --author
              with -l, print the author of each file

 Manual page ls(1) line 1 (press h for help or q to quit)

```

---

- `apropos` - Display Appropriate Commands

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ apropos copy            
cifsdd (8)           - convert and copy a file over SMB
COPY (7)             - copy data between a file and a table
cp (1)               - copy files and directories
cpgr (8)             - copy with locking the given file to the password or group file
cpio (1)             - copy files to and from archives
cppw (8)             - copy with locking the given file to the password or group file
dd (1)               - convert and copy a file
debconf-copydb (1)   - copy a debconf database
git-checkout-index (1) - Copy files from the index to the working tree
gvfs-copy (1)        - Deprecated equivalent of gio copy
install (1)          - copy files and set attributes
mariadb-hotcopy (1)  - a database backup program
mysqlhotcopy (1)     - a database backup program
ntfscp (8)           - copy file to an NTFS volume.
objcopy (1)          - copy and translate object files
ptrepack (1)         - Copy any PyTables Leaf, Group or complete subtree into anothe...
rcp (1)              - OpenSSH secure file copy
rsync (1)            - a fast, versatile, remote (and local) file-copying tool
scp (1)              - OpenSSH secure file copy
ssh-copy-id (1)      - use locally available keys to authorise logins on a remote ma...
svnversion (1)       - Produce a compact version identifier for a working copy.
vfs_shadow_copy (8)  - Expose snapshots to Windows clients as shadow copies.
vfs_shadow_copy2 (8) - Expose snapshots to Windows clients as shadow copies.
x86_64-linux-gnu-objcopy (1) - copy and translate object files
                                                                                       
```

---

- `whatis` : Display One-line Manual Page Descriptions

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ whatis rm    
rm (1)               - remove files or directories
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ whatis ls
ls (1)               - list directory contents
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ whatis sudo
sudo (8)             - execute a command as another user
                            
```

---

- `info` : Display a Program’s Info Entry

```
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ info ls

```

```
Next: dir invocation,  Up: Directory listing

10.1 ‘ls’: List directory contents
==================================

The ‘ls’ program lists information about files (of any type, including
directories).  Options and file arguments can be intermixed arbitrarily,
as usual.

   For non-option command-line arguments that are directories, by
default ‘ls’ lists the contents of directories, not recursively, and
omitting files with names beginning with ‘.’.  For other non-option
arguments, by default ‘ls’ lists just the file name.  If no non-option
argument is specified, ‘ls’ operates on the current directory, acting as
if it had been invoked with a single argument of ‘.’.

   By default, the output is sorted alphabetically, according to the
locale settings in effect.(1)  If standard output is a terminal, the
output is in columns (sorted vertically) and control characters are
output as question marks; otherwise, the output is listed one per line
and control characters are output as-is.

-----Info: (coreutils)ls invocation, 56 lines --Top------------------------------------
Follow xref: gument is specified, ‘ls’ operates on the current directory, acting asif 
```

---

- `alias` : Creating Our Own Commands with alias
    - `trick: It’s possible to put more than one command on a line by separating each command with a semicolon`
    - `command1; command2; command3...`

```
[me@linuxbox ~]$ cd /usr; ls; cd -
bin  games  include  lib  local  sbin  share  src
/home/me
[me@linuxbox ~]$
```
```
[me@linuxbox ~]$ type foo
bash: type: foo: not found
```
```
[me@linuxbox ~]$ alias foo='cd /usr; ls; cd -'
[me@linuxbox ~]$ foo
bin  games  include  lib  local  sbin  share  src
/home/me
[me@linuxbox ~]$
[me@linuxbox ~]$ type foo
foo is aliased to `cd /usr; ls; cd -'
```
```
[me@linuxbox ~]$ unalias foo
[me@linuxbox ~]$ type foo
bash: type: foo: not found
```

---

## 𝐑𝐞𝐝𝐢𝐫𝐞𝐜𝐭𝐢𝐨𝐧

- `<command> > <file>` : Redirecting Standard Output

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ ls -l /usr/bin > ls-output.txt
                                                                                       
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ ls -l                         
total 180
drwxr-xr-x 2 shreyas shreyas   4096 Jan  4 17:21 dir1
drwxr-xr-x 2 shreyas shreyas   4096 Jan  4 17:21 dir2
drwxr-xr-x 2 shreyas shreyas   4096 Jan  4 17:21 dir3
-rw-r--r-- 1 shreyas shreyas 171639 Jan  4 18:21 ls-output.txt
                                                                   
```

---

- `command >> file` - append redirected output to a file instead of overwriting the file

```
[me@linuxbox ~]$ ls -l /usr/bin >> ls-output.txt
```

---

- `0>` OR `<` : redirecting standard input
- `>` : redirecting standard output
- `2>` : redirecting standard error

```
[me@linuxbox ~]$ ls -l /bin/usr 2> ls-error.txt
```

---

- `ls -l /bin/usr > ls-output.txt 2>&1` OR ` ls -l /bin/usr &> ls-output.txt`: Redirecting Standard Output and Standard Error to One File
- `ls -l /bin/usr 2> /dev/null` : Disposing unwanted output

---

- `command1 | command2` : Pipeline
- `wc` : Print line, Word, and Byte counts
- `grep` : print line matching pattern
- `head -n <number of lines> ls-output.txt` : print initial lines of file
- `tail -n <number of lines> ls-output.txt` : print last lines of files 
- `tee` : Read from Stdin and Output to Stdout and Files
- 

```
┌──(shreyas㉿kali)-[~/practise/commandline]
└─$ wc ls-output.txt 
  2557  24294 171639 ls-output.txt

```
```
[me@linuxbox ~]$ head -n 5 ls-output.txt
total 343496
-rwxr-xr-x 1 root root       31316 2017-12-05 08:58 [
-rwxr-xr-x 1 root root        8240 2017-12-09 13:39 411toppm
-rwxr-xr-x 1 root root      111276 2017-11-26 14:27 a2p
-rwxr-xr-x 1 root root       25368 2016-10-06 20:16 a52dec
[me@linuxbox ~]$ tail -n 5 ls-output.txt
-rwxr-xr-x 1 root root        5234 2017-06-27 10:56 znew
-rwxr-xr-x 1 root root         691 2015-09-10 04:21 zonetab2pot.py
-rw-r--r-- 1 root root         930 2017-11-01 12:23 zonetab2pot.pyc
-rw-r--r-- 1 root root         930 2017-11-01 12:23 zonetab2pot.pyo
lrwxrwxrwx 1 root root           6 2016-01-31 05:22 zsoelim -> soelim
```

---

## 𝐒𝐞𝐞𝐢𝐧𝐠 𝐭𝐡𝐞 𝐰𝐨𝐫𝐥𝐝 𝐚𝐬 𝐭𝐡𝐞 𝐬𝐡𝐞𝐥𝐥 𝐬𝐞𝐞𝐬 𝐢𝐭

- `echo` : Display a line of text
    - `echo *` : works same as `ls`
    - `echo D*` : Display files/directories which starts with D
    - `echo *s` : Display files/drectories which ends with s
    - `echo [[:upper:]]*` : Display files/directories that starts with uppercase letters 
    - `echo /usr/*/share` : display all directories between /usr/ & /share
    - `echo ~` : tilde expansion

```
┌──(shreyas㉿kali)-[~]
└─$ echo hello there my name is shreyas                       
hello there my name is shreyas
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo *                             
BugBounty Desktop Documents Downloads Music Pictures practise Public Templates Videos
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo D*
Desktop Documents Downloads
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo *s
Documents Downloads Pictures Templates Videos
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo [[:upper:]]*
BugBounty Desktop Documents Downloads Music Pictures Public Templates Videos
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo /usr/*/share
/usr/local/share
                                                                                      
┌──(shreyas㉿kali)-[~]
└─$ echo ~           
/home/shreyas

                                                                                       
```

- Arithmetic Expansion:
    - `$((expression))` 
   
```                                                                                      
┌──(shreyas㉿kali)-[~]
└─$ echo $((2 + 2))
4

┌──(shreyas㉿kali)-[~]
└─$ echo $(($((5**2)) * 3))
75
      
```

Operator | Description
--- | ---
`+` | Addition
`-` | Subtraction
`*` | Multiplication
`/` | Division (but remember, since expansion supports only integer arithmetic, results are integers)
`%` | Modulo, which simply means “remainder”
`**` | Exponentiation

- Brace Expansion: create multiple text strings from a pattern containing braces

```
┌──(shreyas㉿kali)-[~]
└─$ echo Front-{A,B,C}-Back
Front-A-Back Front-B-Back Front-C-Back
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$  echo Number_{1..5}
Number_1 Number_2 Number_3 Number_4 Number_5
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo {01..15}
01 02 03 04 05 06 07 08 09 10 11 12 13 14 15
                                                                                       
┌──(shreyas㉿kali)-[~]
└─$ echo a{A{1,2},B{3,4}}b
aA1b aA2b aB3b aB4b
                                                   
```

- Parameter expansion: `echo $var`
- Command Substitution
    -  `echo $(ls)`
    -  `ls -l $(which cp)`
    -  `file $(ls -d /usr/bin/* | grep zip)`
   
---

- Quoting:
    - Double Quotes: If we place text inside double quotes, all the special characters used by the shell lose their special meaning and are treated as ordinary characters. The exceptions are $ (dollar sign), \ (backslash), and ` (backtick).
    - Single Quotes: If we need to suppress all expansions, we use single quotes.
- Escaping Characters:
    - `\` : is used for escaping
- Backslash Escape Situation:

Escape Sequence | Meaning
--- | ---
`\a` | Bell (an alert that causes the computer to beep)
`\b` | Backspace
`\n` | Newline; on Unix-like systems, this produces a line feed
`\r` | Carriage return
`\t` | tab

```
┌──(shreyas㉿kali)-[~]
└─$ sleep 10; echo -e "Time's up\a"
Time's up
           
```
---

## 𝐀𝐝𝐯𝐚𝐧𝐜𝐞𝐝 𝐊𝐞𝐲𝐛𝐨𝐚𝐫𝐝 𝐓𝐫𝐢𝐜𝐤𝐬

- `clear` : Clear the terminal screen
- `history` : Display or manipulate the history list

- Cursor Movement:

Key | Action
--- | ---
`CTRL-A` | Move the cursor to the beginning of line
`CTRL-E` | Move cursor to the end of the line
`CTRL-F` | Move cursor forward one character; same as the right arrow key
`CTRL-B` | Move cursor backward one character; same as the left arrow key
`ALT-F` | Move cursor one word forward
`ALT-B` | Move cursor backward one word
`CTRL-L` | Clear screen and move the cursor to the top left corner. Same as `clear` command

---
- Modifying Text


Key | Action
--- | ---
`CTRL-D` | Delete the character at the cursor location
`CTRL-T` | Transpose the character at the cursor location
`ALT-T` | Transpose the word at the cursor location with the one preceding it.
`ALT-L` | Convert the characters from the cursor location to the end of the word to lowercase.
`ALT-U` | Convert the characters from the cursor location to the end of the word to uppercase.

---

- History Expansion

Sequence | Action
--- | ---
`!!` | Repeat the last command. It is probably easier to press the up arrow and ENTER
`!number` | Repeat history list item `number`.
`!string` | Repeat last history list item starting with `string`
`!?string` | Repeat last history list item containing  `string`


---

## 𝐏𝐞𝐫𝐦𝐢𝐬𝐬𝐢𝐨𝐧𝐬

- `id` : Display user identity
- `chmod` : Change a file’s mode
- `umask` : Set the default file permissions
- `su` : Run a shell as another user
- `sudo` : Execute a command as another user
- `chown`: Change a file’s owner
- `chgrp`: Change a file’s group ownership
- `passwd`: Change a user’s password

- Permission attribute Examples:

File Attributes | Meaning
--- | ---
`-rwx------` | A regular file that is readable, writable, and executable by the file’s owner. No one else has any access.
`-rw-------` | A regular file that is readable and writable by the file’s owner. No one else has any access.
`-rw-r--r--` | A regular file that is readable and writable by the file’s owner. Members of the file’s owner group may read the file. The file is world-readable.
`-rwxr-xr-x` | A regular file that is readable, writable, and executable by the file’s owner. The file may be read and executed by everybody else.
`-rw-rw----` | A regular file that is readable and writable by the file’s owner and members of the file’s group owner only.
`lrwxrwxrwx` | A symbolic link. All symbolic links have “dummy” permissions. The real permissions are kept with the actual file pointed to by the symbolic link.
`drwxrwx---` | A directory. The owner and the members of the owner group may enter the directory and create, rename, and remove files within the directory.
`drwxr-x---` | A directory. The owner may enter the directory and create, rename, and delete files within the directory. Members of the owner group may enter the directory but cannot create, delete, or rename files.

---

- `chmod` : Change File Mode
    - 6(rw-)
    - 7(rwx)
    - 5(r-x)
    - 4(r--)
    - 0(---)
    
Symbol | Meaning
--- | ---
`u` | Short for "user" but means the file or directory owner.
`g` | Group owner
`o` | Short for "others" but means world
`a` | Short for "all". This is a combination of `u`, `g`, and `o`.

- If no character is specified, “all” will be assumed. The operation may be a + indicating that a permission is to be added, a - indicating that a permission is to be taken away, or a = indicating that only the specified permissions are to be applied and that all others are to be removed.

Notation | Meaning
--- | ---
`u+x` | Add execute permission for the owner.
`u-x` | Remove execute permission from the owner.
`+x` | Add execute permission for the owner, group, and world. This is equivalent to a+x.
`o-rw` | Remove the read and write permissions from anyone besides the owner and group owner.
`go=rw` | Set the group owner and anyone besides the owner to have read and write permissions. If either the group owner or the world previously had execute permission, it is removed.
`u+x,go=rx` | Add execute permission for the owner and set the permissions for the group and others to read and execute. Multiple specifications may be separated by commas.

---

## 𝐏𝐫𝐨𝐜𝐞𝐬𝐬𝐞𝐬

- `ps` : Report a snapshot of current processes
- `top` : Display tasks
- `jobs` : List active jobs
- `bg` : Place a job in the background
- `fg` : Place a job in the foreground
- `kill` : Send a signal to a process
- `killall` : Kill process by name
- `shutdown` : Shut down or reboot the system





