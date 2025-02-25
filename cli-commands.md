### COMMANDS

jq - use for all sorts
https://jqlang.github.io/jq/download/
https://www.youtube.com/watch?v=n8sOmEe2SDg


history - show last 1000 commands
ctrl + l - same as  clear

https://deepu.tech/rust-terminal-tools-linux-mac-windows-fish-zsh/
kdash - open kubernetes moniter
br - new way of navigating (ctrl + -> for preview) - https://github.com/Canop/broot
fzf - fuzzy find in dir
c - clear screen
btm - system moniter
topgrade - update all system componants
**grep on multi-core steroids**
ag --ts {searchterm} 
rg {searchterm} (ripgrep)
n (neovim)
b/bat (better cat)
rip (rm, rip -u can undo any delete!)
z {locaiton} - cd alternative
dust - disk usage
### COMMAND LINE


C - b - open this document!
C - i - open chtsh script
C - l - run tmux launcher
C - f - run tmux sessionizer
C - r - run fzf
C - d - EOF signal, close recursively

tldr {subject name} - gives output od most common commands - short version of man cli tool. eg: tldr git worktree
ccat - coloured output file
man man - manual for how to use manuals
man (app) - manual for app, eg man tmux - example: man git worktree
cht.sh - cheat sheet cli
/tmp/ - error log dir - use cat for items in here. use bash to help log debug info

------------------------------------------------------------------------------------


### GITHUB COPILOT

<Tab> Accept current suggestion.
<C-]> Dismiss the current suggestion. (ctrl)
<M-]> Cycle to the next suggestion, if one is available. (alt)
<M-[> Cycle to the previous suggestion. (alt)
<M-\> Explicitly request a suggestion, even if Copilot is disabled. (alt)
:Copilot disable 

### TMUX (all have ctrl + a prefix, unless stated otherwise)

shift + d - look for a todo.md in current dir, create one if not. Make notes where you are
ctrl + d - end of file signal, recusively close tmux upwards
tmux ls - list all sessions i

PREFIX + [ - ENABLE SCROLLBACK, up, down etc to navigate or vim keybinds
PREFIX + i - OPEN CHEATSHEET
PREFIX + l - GO TO PREVIOUS SESSION!
PREFIX + w - OPEN SESSION/WINDOW NAVIGATION
PREFIX + c - new window
PREFIX + p - previous window
PREFIX + n - next window

man tmux - show manual (man man - shows how to use manual)

Alias 		Command 			Description
ta "some name" 	tmux attach -t 			Attach to already running named session
tad "some name" tmux attach -d -t 		Detach named tmux session
ts "some name" 	tmux new-session -s 		Create a new named tmux session
tl 		tmux list-sessions 		Displays a list of running tmux sessions
tksv 		tmux kill-server 		Terminate all running tmux sessions
tkss 		tmux kill-session -t 		Terminate named running tmux session
tmux 		_zsh_tmux_plugin_run 		Start a new tmux session
tmuxconf 	$EDITOR $ZSH_TMUX_CONFIG 	Open .tmux.conf file with an editor

## Sessions (no prefix)

tmux new-session -d -n "some name" - creates new detached session
tl - list sessions

# Navigation

shift + 9 - (open parethesis) navigate left session
shift + 0 - (close parenthesis) navigate right session

## Windows

w - show/navigate between windows in a session
c - new window

# Navigation

n - next window
p - previous window
(# number) - for window number

## CLI comms
tmux new-window - creates new window in attached session 

ta 	tmux attach -t 	Attach new tmux session to already running named session
tad 	tmux attach -d -t 	Detach named tmux session
ts 	tmux new-session -s 	Create a new named tmux session
tl 	tmux list-sessions 	Displays a list of running tmux sessions
tksv 	tmux kill-server 	Terminate all running tmux sessions
tkss 	tmux kill-session -t 	Terminate named running tmux session

## MANUAL SESSION MANAGEMENT (currently auto saves every 15mins)

Save: Press Ctrl-b (or your custom prefix key), then while holding Ctrl, press s.
Restore: Press Ctrl-b (or your custom prefix key), then while holding Ctrl, press r.!

--------------------------------------------------------------------------------------------

### NEOVIM

A file - not what we edit - we work on buffers, which can then be written to the file
Buffers - represent a change to the file in memory. 
Window - a view into the buffer. These can close and the buffer can remain in memory
Tabs - another viewport, can be many windows and splits per tab
Splits - splits of a viewport into n sections
(we cam)

:h {name} - get help with whatever topic in split view, eg :h buffer
 -> :q to close help file

:new - new split (horizontal)
:vnew - new split (vertical)

MOTION - anything that moves your cursor   



