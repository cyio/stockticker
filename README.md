## What does it do?

This is a script you could use to display stock pre-market price in your tmux status line

## How to use it?

### install
npm install -g stockticker

### usage
stockticker NASDAQ:APAPL

### tmux config

add following to your tmux config (assuming ~/.tmux.conf)

```
set -g status-fg green
set -g status-bg black
set -g status-attr bright
set-window-option -g window-status-current-bg green
set-window-option -g window-status-current-fg black
set-window-option -g window-status-current-attr dim
set -g status-right '#[fg=cyan,bright]#(biticker NASDAQ:AAPL)'
set -g status-right-length 75
set status-interval 60
```

then run 

```
tmux source-file ~/.tmux.conf
```

## Donate

:)

```
1JMQVCZgXD1Ejr49MouHqifJMjPgmnMrv7
```
