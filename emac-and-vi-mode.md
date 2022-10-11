## 𝐄𝐦𝐚𝐜𝐬 𝐚𝐧𝐝 𝐕𝐢 𝐦𝐨𝐝𝐞𝐬 𝐢𝐧 𝐁𝐚𝐬𝐡


- Emacs Mode
> - This is usually the default editing mode when in the bash environment and means that you are able to use commands like those in Emacs (defined in the Readline library) to move the cursor, cut and paste text, or undo editing.
```
$ set -o emacs
```

> - Keyboard shortcuts:

```
ctrl-a Move cursor to beginning of line
ctrl-e Move cursor to end of line
meta-b Move cursor back one word
meta-f Move cursor forward one word
ctrl-w Cut the last word
ctrl-u Cut everything before the cursor
ctrl-k Cut everything after the cursor
ctrl-y Paste the last thing to be cut
ctrl-_ Undo
NOTE: ctrl- = hold control, meta- = hold meta (where meta is usually the alt or escape key).
A combination of ctrl-u to cut the line combined with ctrl-y can be very helpful. If you are in middle of typing a command and need to return to the prompt to retrieve more information you can use ctrl-u to save what you have typed in and after you retrieve the needed information ctrl-y will recover what was cut.

```

---

- Vi Mode
> - Vi mode allows for the use of vi like commands when at the bash prompt. When set to this mode initially you will be in insert mode (be able to type at the prompt unlike when you enter vi). Hitting the escape key takes you into command mode.

```
$ set -o vi
```
> - Keyboard Shortcuts:

```
h Move cursor left
l Move cursor right
A Move cursor to end of line and put in insert mode
0 (zero) Move cursor to beginning of line (doesn't put in insert mode)
i Put into insert mode at current position
a Put into insert mode after current position
dd Delete line (saved for pasting)
D Delete text after current cursor position (saved for pasting)
p Paste text that was deleted
j Move up through history commands
k Move down through history commands
u Undo
```

---
> - Suggested by: [GoldenCeks](https://www.reddit.com/r/HowToHack/comments/y0cu5t/comment/irtehdm/?utm_source=share&utm_medium=web2x&context=3) 
> - Reference: [set-o-vi-emacs](https://mywiki.wooledge.org/set-o-vi-emacs)
> - Done
