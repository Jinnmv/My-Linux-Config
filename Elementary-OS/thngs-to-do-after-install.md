
# Update
First thing 
```
sudo apt-get update
sudo apt-get dist-upgrade
```

# Keyboard Layout

It's known issue that there are several issues with keyboard layouts support. For now dirty workaround could be used to get this worked.
1. Ensure more than one layout added (TBD)
2. Clear standard layout swithc shortcut (TBD)

Open 

```
gsettings set org.pantheon.desktop.gala.keybindings switch-input-source "['<Alt>Shift_L', '<Alt>Shift_R', '<Shift>Alt_L', '<Shift>Alt_R', '<Ctrl>Shift_L', '<Ctrl>Shift_R', '<Shift>Control_L', '<Shift>Control_R']"
```

Remove unneeded shortcuts

# 256 colors in terminal
There are two ways to have 256 colors supported in terminal
1. dconf
2. .bashrc, TERM=xterm-256color

http://www.elementarynow.com/what-is-elementary-3/things-to-do/
http://linuxscoop.com/video/20-things-to-do-after-installing-elementary-os-freya
