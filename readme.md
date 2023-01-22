# XFCE4 Rice for MacBook Pro 2012

## Extra Recommended Configuration

### Removing Snaps (if using Xubuntu)

To install Firefox as a .deb:  
https://www.omgubuntu.co.uk/2022/04/how-to-install-firefox-deb-apt-ubuntu-22-04

Then remove all Snaps and Snapd:  
https://askubuntu.com/questions/1309144/how-do-i-remove-all-snaps-and-snapd-pre>

### Configure Trackpad

`sudo cp 60-synaptics-options.conf /etc/X11/xorg.conf.d/60-synaptics-options.conf`

Inverts trackpad scroll, reduces sensitivity a little and turns on palm rejection.

### Change xcape bindings from Ctrl+Escape to Alt+F1

`sudo cp xcape-super-bindings.desktop /etc/xdg/xdg-xubuntu/autostart/`

This is necessary otherwise the next step to swap Esc and CapsLock will break the Super Key

### Swap Esc and CapsLock

`setxkbmap -option caps:swapescape`

### Change Eject Key to Delete

`sudo cp 65-keyboard-custom.hwdb /lib/udev/hwdb.d/`
`sudo systemd-hwdm update`

Credit to the guy here who made a really good post about this:  
https://askubuntu.com/questions/1019276/fake-key-code-for-remapped-keyboard-keys/1019659#1019659
