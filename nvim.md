# Neovim Cheatsheet

## Basic Horizontal Motions

[hjkl] = move cursor: left (h), down (j), up (k), right (l)
w = move to the next word
b = move backward to the previous word
0 = move to the beginning of the current line
^ = move to the first non-blank character on the current line
$ = move to the end of the current line

## Basic Vertical Motions

gg = move to the first line of the current buffer
Shift+g = move to the last line of the current buffer
<number> gg = move at line <number>
% = move to the matching bracket

## From NORMAL to INSERT mode and back

i = switch to INSERT mode before the character under the cursor
a = switch to INSERT mode after the character under the cursor
I = switch to INSERT mode before the beginning of the current line
A = switch to INSERT mode after the end of the current line
o = open a new line below the current one, and switch to INSERT mode
O = open a new line above the current one, and switch to INSERT mode
Esc = switch back to NORMAL mode

## Scrolling

Ctrl+u = move half a screen upward
Ctrl+d = move half a screen downward

## Undo and Redo

u = undo
Ctrl+r = redo

## Operators

d = delete
c = change
y = yank (copy)

### Examples of Text Objects

diw = delete inside word
ciw = change inside word
caw = change a word
ci' = change inside '

## Creating and Navigating Windows

Ctrl+[hjkl] = navigate windows: left (h), down (j), up (k), right (l)
Ctrl+w v = split vertically the current window
Ctrl+w h = split horizontally the current window

## Resizing and Moving Windows

Ctrl+w r = rotate the windows
Ctrl+w x = exchange the focused window with the next window
Ctrl+w [-+] = decrease (-) or increase (+) window's height
Ctrl+w [<>] = decrease (<) or increase (>) window's width
Ctrl+w = = resize windows equally for them to fit the screen

## Change list

- g; = jump to the next change
- g, = jump to the previous change

## Method jump

- [m = move to the start of a method
- ]m = move to the end of a method

## Writing Buffers and Closing Windows

:w = write the current buffer into the file
:q = quit the current window, close Neovim if there is no more window open
:q! = quit the current window, and ignore the buffer's modifications
:qa = quit all the windows (add ! to ignore buffers' modifications)
:wqa = quit and write all the windows

## The command window

- q: = open the command history
- q/ and q? = open the search history
- <c-f> = open the command history while in command-line mode

## coc.nvim

<!-- - <space-a> = show diagnostics -->
<!-- - <space-o> = show symbols in a file -->
<!-- - <space-s> = search symbols in a workspace -->

## gv.vim

- `:GV` = open commit browser
- `:GV!` = only list commits that affected the current file
- `:GV?` = fills the location list with the revisions of the current file
- `o` or `<cr>` (on a commit) = display the content of it
- `o` or `<cr>` (on commits) = display the diff in the range
- `O` = open a new tab instead
- `.` = start command-line with `:Git [CURSOR] SHA` a la fugitive
- `q` or `gq` = close
    
## netrw

:Vexplore = opens netrw in a vertical split

## vim-gitgutter

- [c = go to previous hunk
- ]c = go to next hunk
- <leader>hp = preview hunk
- <leader>hs = stage hunk
- <leader>hu = undo hunk
