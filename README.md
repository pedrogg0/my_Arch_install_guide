# my_kali_install-config
I will save here my install and config of kali in virtualbox

# Installation

I downloaded it from https://www.kali.org/get-kali/#kali-virtual-machines picked virtual box version cause vmware version was causing me troubles with keyboard unrecognition

I just imported it with virtual box and updated the system after startup.

I changed the keyboard layout with: setxkbmap -layout es  //to-do run it at start

# i3wm Installation

sudo apt-install i3-gaps

## changing screen scale 

echo "Xft.dpi: 150" > ~/.Xresources

xrdb -merge ~/.Xresources
exec i3

## i3wm Themes installation 

I will use: https://github.com/stav121/i3wm-themer //crashed  

//to-do install a windows manager
