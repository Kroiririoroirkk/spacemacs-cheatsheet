# Spacemacs Cheatsheet
Author: Eric Tao

## Movement
* `h` – left
* `l` – right
* `b` – move backward by word
* `w` – move forward by word
* `t<character>` – move forward to right before first occurrence of `<character>`
* `f<character>` – move forward to first occurrence of `<character>`
* `j` – down
* `k` – up
* `C-d` – jump down (half page)
* `C-u` – jump up (half page)
* `gg` – first line
* `G` – last line
* `}` – down one paragraph
* `{` – up one paragraph
* `^` – start of line (non-whitespace)
* `0` – start of line
* `$` – end of line

## Edit
* `i` – insert
* `ESC` or `fd` – switch to normal state
* `a` – append
* `I` – insert at the beginning of the line
* `A` – add to end of line
* `u` – undo
* `C-r` – redo
* `SPC i j` – new indented line below
* `SPC i k` – new indented line above
* `SPC i J` – new line below
* `SPC i K` – new line above
* `o` – new line below and go to insert mode
* `O` – new line above and go to insert mode
* `.` – repeat last edit command
* `<number>.` – repeat last edit command `<number>` times

## Cut and paste
* `v` – enter visual character mode (highlight)
* `V` – enter visual line mode (highlight)
* `C-v` – enter visual block mode (highlight)
* `v $` – highlight until end of line
* `C-x h` – highlight everything
* `y` – yank (copy) text
* `y y` – yank (copy) current line
* `y w` – yank (copy) current word
* `d` – cut
* `d d` – cut whole line
* `d w` – cut whole word
* `c` – cut then insert
* `c c` – cut whole line then insert mode
* `c w` – cut whole word then insert mode
* `x` – cut current character
* `p` – paste
* `P` – paste before
* `[ P` – paste in newline above
* `] P` – paste in newline below
* `>` – increase indentation (tap twice when no text is highlighted)
* `<` – decrease indentation (tap twice when no text is highlighted)

## Search
* `/<pattern> RET` – Forward search `<pattern>`
* `?<pattern> RET` – Backward search `<pattern>`
* `*` – Next occurrence of word under cursor
* `#` – Previous occurrence of word under cursor
* `:%s/<old>/<new>/g RET` – Replace every `<old>` for `<new>` in whole buffer
* `:%s/<old>/<new>/gc RET` – Replace every `<old>` for `<new>` in whole buffer (confirm each time)

## File
* `SPC f f` – new file or open file
* `SPC f s` – save file
* `SPC f R` – rename file
* `SPC f d` – delete file

## Program
* `SPC q q` – quit
* `SPC q r` – restart
* `SPC f e d` – open `.spacemacs`
* `SPC f e R` – apply changes to `.spacemacs`
* `:!` – execute shell command
* `SPC ?` – search through key bindings in current major mode

## Frames and windows
* `SPC F n` – create a new frame
* `SPC F d` – delete frame
* `SPC F D` – delete all other frames
* `SPC w -` – split window into two pieces vertically
* `SPC w /` – split window into two pieces horizontally
* `SPC w |` – make only vertical window and maximize
* `SPC w _` – make only horizontal window and maximize
* `SPC w u` – undo last change to windows
* `SPC w U` – redo last change to windows
* `SPC w d` – delete window
* `SPC w m` – maximize current window (or undo maximization)
* `SPC w w` – cycle between windows
* `SPC w j/k/h/l` – switch to window up/down/left/right
* `SPC w J/K/H/L` – move window up/down/left/right
* `SPC <number>` – switch to window number `<number>`
* `SPC TAB` – go to previous buffer visited by window
* `q` – quit a buffer (in many different settings)

## Git
* `SPC g i` – git init
* `SPC g c` – git clone
* `SPC g s` – open a status buffer
* `h` in status buffer – help
* `s` in status buffer – stage a file
* `S` in status buffer – stage all
* `u` in status buffer – unstage a file
* `U` in status buffer – unstage all
* `M` in status buffer – remote (can paste URL with C-y)
* `b` in status buffer – branch
* `p` in status buffer – push
* `F` in status buffer – pull
* `c` in status buffer – commit
* `, c` in commit buffer - confirm and quit commit message
* `, a` in commit buffer – abort and quit commit message

## Markdown
* `, c p` – preview
* `, c P` – enable/disable live preview mode

## Python
* `, =` – reformat buffer
* `, c c` – execute current file
* `, '` – start Python
* `, v a` – activate virtual environment
* `, v d` – deactivate virtual environment
* `, g a` – go to a variable assignment
* `, g b` – go back
* `, h h` – quick documentation
* `, S d` – insert docstring skeleton using sphinx-doc
* `, r f` – fix missing import statement with importmagic
* `, r i` – remove unused imports with autoflake
* `, r I` – sort imports with isort
* `C-c <` – de-indent one layer
* `C-c >` – indent one layer
