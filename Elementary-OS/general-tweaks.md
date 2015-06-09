
# Plank

## Folder view for plank:

1. open $HOME/.config/plank/dock1
2. create a file, in $HOME/.config/plank/dock1/launchers. e.g.: home_folder.dockitem
3. put next lines to the file:

  ```
  [PlankItemsDockItemPreferences]
  Launcher=/path/to/your/folder
  ```
  
  save changes
  
## Add new menu-items for Plank launchers

Let's use `xfce4-terminal` for instance

Open `/usr/share/applications/xfce4-terminal.desktop` and put these lines to the end:

```
Actions=NewWindow;NewTab;NewDropDown;NewFullscreen

[Desktop Action NewWindow]
Name=Open a New Terminal
Exec=xfce4-terminal --window
OnlyShowIn=Unity;

[Desktop Action NewTab]
Name=Open a New Tab
Exec=xfce4-terminal --tab
OnlyShowIn=Unity;

[Desktop Action NewDropDown]
Name=Open a New DropDown Terminal
Exec=xfce4-terminal --drop-down
OnlyShowIn=Unity;

[Desktop Action NewFullscreen]
Name=Open a New Fullscreen Terminal
Exec=xfce4-terminal --fullscreen
OnlyShowIn=Unity;
```

save
