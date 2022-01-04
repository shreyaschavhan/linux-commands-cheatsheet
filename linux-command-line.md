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




