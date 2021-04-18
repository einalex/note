# note
Script that turns selected text into a note file (nextcloud notes compatible) 

![Screenshot usage example of note](https://github.com/einalex/note/blob/main/note.png)

### features
* rofi-based UI
* add the selected text to existing notes
* editable note title
* suggests a date/time based title for taking notes without further thought

### prerequesits
* bash (should be preinstalled on your box)
* rofi
* xclip (should be preinstalled on your box if using an X window environment)

### installation
1. make it executable `chmod +x note`
2. move the script to a folder in your PATH `mv note ~/.local/bin/`
3. adjust the TARGET_FOLDER variable inside the script file to match your setup
4. add a keybinding to your desktop environment to run the script

### i3wm integration
1. edit your i3 config file `~/.config/i3/config`
2. add `bindsym $mod+n exec note`

### nextcloud integration
1. install nextcloud client
2. adjust TARGET_FOLDER variable to some subfolder of `LOCAL_NEXTCLOUD_ROOT/Notes`


### Zettelkasten time format
adjust the `date +Iseconds` part to be `date +%Y%m%e%H%M%S`
