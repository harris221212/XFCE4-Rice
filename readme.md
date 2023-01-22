# XFCE4 Rice for MacBook Pro 2012

# Extra Recommended Configuration

## Removing Snaps (if using Xubuntu)

To install Firefox as a .deb: 
`https://www.omgubuntu.co.uk/2022/04/how-to-install-firefox-deb-apt-ubuntu-22-04`

Then remove all Snaps and Snapd:
`https://askubuntu.com/questions/1309144/how-do-i-remove-all-snaps-and-snapd-pre>`

## Configure Trackpad

`sudo cp 60-synaptics-options.conf /etc/X11/xorg.conf.d/60-synaptics-options.conf`

Inverts trackpad scroll, reduces sensitivity a little and turns on palm rejection.
