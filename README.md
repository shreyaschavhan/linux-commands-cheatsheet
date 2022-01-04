# ⁍ 𝐋𝐢𝐧𝐮𝐱 𝐂𝐨𝐦𝐦𝐚𝐧𝐝𝐬 𝐂𝐡𝐞𝐚𝐭𝐬𝐡𝐞𝐞𝐭

Command | Usage 
:-: | ---
`ssh` | ssh (SSH client) is a program for logging into a remote machine and for executing commands on a remote machine.  
`ls` | List  information  about  the FILEs (the current directory by default).
`cd` | Change Directory
`cat` | Concatenate files and print on the standard output
`file` | determine file type
`du` | estimate file space usage
`find`| search for files in a directory hierarchy
`grep` | print lines that match patterns
`sort` | sort lines of text files
`uniq` | report or omit repeated lines
`strings` | print the sequences of printable characters in files
`base64` | base64 encode/decode data and print to standard output
`tr` | Translate, squeeze, and/or delete characters from standard input, writing to standard output.
`tar` | an archiving utility
`gzip` | compress or expand files
`bzip2` | a block-sorting file compressor
`xxd` | make a hexdump or do the reverse.
`mkdir` | make directories
`cp` | copy files and directories
`mv` | move files and directories
`telnet` | The telnet command is used for interactive communication with another host using the TELNET protocol
`nc` | netcat is a simple unix utility which reads and writes data across network connections, using TCP or UDP protocol.
`openssl` | OpenSSL command line tool
`s_client` | The s_client command implements a generic SSL/TLS client which connects to a remote host using SSL/TLS. It is a very useful diagnostic tool for SSL servers.
`nmap` | Network exploration tool and security / port scanner
`diff` | compare files line by line
`bash` | Bash  is  an  sh-compatible  command language interpreter
`screen` | Screen is a full-screen window manager that multiplexes a physical terminal between several processes
`tmux` | tmux is a terminal multiplexer: it enables a number of terminals to be created, accessed, and controlled from a single screen. 
`bg` | background a process
`fg` | foreground a process
`jobs` | list processes running in background
`&` | run a command in background
`cron` |  daemon to execute scheduled commands
`crontab` | maintain crontab files for individual users
`crontab(5)` | tables for driving cron
`more` | file perusal filter for crt viewing
`less` | opposite of more
`vi` | vim - Vi IMproved, a programmer's text editor
`id` | print real and effective user and group IDs
`pwd` | print working directory
`git` | the stupid content tracker
`locate` | find files by name, quickly
`man` | an interface to the system reference manuals
`which` | locate a command
`type` | lets you query the type of each command.
`ps` | report a snapshot of the current processes.
`kill` | send a signal to a process
`uname` | print system information 
`chmod` | change file mode bits
`chown` | change file owner and group
`chgrp` | change group ownership

---

> - cat a file with name "-" : `cat ./-` (./ - stands for current directory) 
> - cat a file whose name starts with "-" : `cat ./-filename`
> - cat a file name with spaces: `cat \spaces \in \this \filename.txt` (Original filename: `spaces in this filename.txt` )
> - base64 decode a file: `base64 -d data.txt`
> - output human readable text from non-humanreadable file: `strings filename`
> - rotate a text with all lowercase and uppercase by 13 positions: `echo "acbdlksjfla KHLKJfdlsfasd" |  tr 'A-Za-z' 'N-ZA-Mn-za-m'`
> - connect a host with ssl encryption: `openssl s_client -connect <host>:<port>`
> - check difference: `diff fileone filetwo`

