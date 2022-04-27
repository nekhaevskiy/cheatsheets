# Neovim cheatsheet

## Windows

- <c-w> v = split the current window vertically
- <c-w> r = rotate the windows

## Change list

- g; = jump to the next change
- g, = jump to the previous change

## Method jump

- [m = move to the start of a method
- ]m = move to the end of a method

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

## vim-gitgutter

- [c = go to previous hunk
- ]c = go to next hunk
- <leader>hp = preview hunk
- <leader>hs = stage hunk
- <leader>hu = undo hunk
