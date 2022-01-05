## 𝐕𝐢𝐦 (𝐕𝐢 𝐈𝐦𝐩𝐫𝐨𝐯𝐞𝐝) 𝐂𝐡𝐞𝐚𝐭𝐬𝐡𝐞𝐞𝐭

- Why to learn Vi?
  - Vi is almost always available. Absolute necessary and good to know for pentesting.
  - Vi is lightweight and fast.

- `vi` : Starting Vi

```
~
~
~                         VIM - Vi Improved
~
~                          version 8.0.707
~                     by Bram Moolenaar et al.
~            Vim is open source and freely distributable
~
~                     Sponsor Vim development!
~          type  :help sponsor<Enter>    for information
~
~          type  :q<Enter>               to exit
~          type  :help<Enter>  or  <F1>  for on-line help
~          type  :help version8<Enter>   for version info
~
~                   Running in Vi compatible mode
~          type  :set nocp<Enter>        for Vim defaults
~          type  :help cp-default<Enter> for info on this
~
~
```

- `:q` : Exiting Vi
- `:q!` : force exiting Vi
- `vim foo.txt` : creating new file and editing using Vi
- `press i` : to enter editing mode
- `press ESC`: to exit insert mode
- `:w` : to save work

- Moving Cursor Around:

Key | Moves the cursor
--- | ---
`l` or `right arrow` | Right one character
`h` or `left arrow` | Left one character
`j` or `down arrow` | Down one line.
`k` or `up arrow` | Up one line
`0 (zero)` | To the beginning of the current line.
`^` | To the first non-whitespace character on the current line
`$` | To the end of the current line
`w` | To the beginning of the next word or punctuation character.
`W` | To the beginning of the next word, ignoring punctuation characters
`b` | To the beginning of the previous word or punctuation character.
`B` | To the beginning of the previous word, ignoring punctuation characters.
`CTRL-F or Page Down` | Down one page
`CTRL-B or PAGE UP` | Up one page
`numberG` | To line number. For example, 1G moves to the first line of the file
`G` | To the last line of the file.


- `u` : undo the last change that you made.
- `a` : append text at the end of the line.
- `o` : Insert line below the current line.
- `O` : Insert line above the current line.
- `x` : will delete a character at the cursor location.

Command | Deletes
--- | ---
`x` | The current character
`3x` | The current character and the next two characters
`dd` | The current line
`5dd` | The current line and the next four lines
`dW` | From the current cursor position to the beginning of the next word
`d$` | From the current cursor location to the end of the current line
`d0` | From the current cursor location to the beginning of the line
`d^` | From the current cursor location to the first non-whitespace character in the line.
`dG` | From the current line to the end of the file
`d20G` | From the current line to the twentieth line of the file

- `y`: is used to yank (copy) text
- `d`: cut the text
- `p`: paste the contents

Command | Copies
---|---
`yy` | The current line
`5yy` | The current line and the next four lines
`yW` | From the current cursor position to the beginning of the next word
`y$` | From the current cursor location to the end of the current line
`y0` | From the current cursor location to the beginning of the line
`y^` | From the current cursor location to the first non-whitespace character in the line
`yG` | From the current line to the end of the file
`y20G` | From the current line to the twentieth line of the file.

- `J (capital j)`: to join lines
- `f`: search within a line
- `/Line`: search within a file
- `:%s/Line/line/g`: global search and replace
- 

