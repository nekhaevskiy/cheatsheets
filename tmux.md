# tmux Cheatsheet

## General

Ctrl+Space = prefix key
Prefix r = reload tmux configuration
Prefix s = list all sessions
Prefix d = detach current session
Prefix : = command prompt

## Panes

Ctrl+[hjkl] = navigate panes
Prefix h = split window horizontally
Prefix v = split window vertically
Prefix Alt+<arrow-key> = resize panes

## Windows

Prefix c = create a new window
Prefix n = rename the current window
Alt+<number> = go to window <number>

## Copy Mode

Prefix [ = enter copy mode
[hjkl] = navigate the shell in copy mode
Ctrl+[ud] = move half a page in copy mode: (u) up, (d) down
/ = search in copy mode
v = selection in copy mode
y = copy selection in copy mode

## Plugins

Prefix Shift+i = install the plugins declared in tmux.conf
Prefix / = regex search (copycat)
Prefix Ctrl+g = jumping over git status files, best used after `git status` command (copycat)
Prefix Alt+h = jumping over SHA-1/SHA-256 hashes (best used after `git log` command (copycat)
Prefix Ctrl+u = url search (copycat)
Prefix Alt+i = ip address search (copycat)
Prefix Tab = select and copy output with fzf (extrakto)
Prefix j = enter the first character of the word and jump to it
