# notes
TMUX and VIM

TMUX Shortcuts
Start new named session
tmux new -s myname

Attach to named
tmux a -t myname

List sessions
tmux ls

Kill session
tmux kill-session -t myname


Panes.. all preceded with ctrl-b
%  vertical split
"  horizontal split
o  swap panes
q  show pane numbers
x  kill pane
+  break pane into window (e.g. to select text by mouse to copy)
-  restore pane from window
⍽  space - toggle between layouts
<prefix> q (Show pane numbers, when the numbers show up type the key to goto that pane)
<prefix> { (Move the current pane left)
<prefix> } (Move the current pane right)
<prefix> z toggle pane zoom

Windows - again precede with ctrl-b
c  create window
w  list windows
n  next window
p  previous window
f  find window
,  name window
&  kill window


VIM
:q        close
:w        write/saves
:wa[!]    write/save all windows [force]
:wq       write/save and close
:x        save and quit, same as wq
:q!       force close if file has changed and not save changes
v        Enter visual mode for selection of LINES
C-v      Enter visual mode for selection of BLOCKS
y        Yank/copy selected region
yy       Yank/copy entire line
"<reg>y  Yank/copy marked region into register <reg> (register from a-z)
c        Cut selection
p        Paste yanked content
"<reg>p  Paste yanked content in register <reg> (from a-z)
P        Paste yanked content BEFORE
u        Undo
C-r      Redo

Navigation
h        cursor left
j        cursor down
l        cursor right
k        cursor up
H        Jump to TOP of screen
M        Jump to MIDDLE of screen
L        Jump to BOTTOM of screen
C-b      Move back one full screen (page up)
C-f      Move forward one full screen (page down)
C-d      Move forward 1/2 screen; half page down
C-u      Move back (up) 1/2 screen; half page up
w        jump by start of words (punctuation considered words)
e        jump to end of words (punctuation considered words)
b        jump backward by words (punctuation considered words)
0 (zero) start of line
^        first non-blank character of line
$        end of line
G        bottom of file
gg       top of file
