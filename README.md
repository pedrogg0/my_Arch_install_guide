# My_Arch_install_guide
I will save here my install and config of Arch linux

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

## i3wm extra utilities installation 

I will use: https://vincent.bernat.ch/en/blog/2021-i3-window-manager 

I installed:
-polybar for making the status bar prettier
-picom as a compositor for transparencies etc
-rofi as app launcher
-feh as desktop wallpaper handler

## i3wm change keyboard layout

setxkbmap -layout es
setxkbmap -option 'grp:alt_shift_toggle'

copied in ~/.config/i3/config:
exec "setxkbmap -layout es"
exec "setxkbmap -option 'grp:alt_shift_toggle'"

## copy i3/config in ~/.config

## rofi config

used https://github.com/adi1090x/rofi#menu

## polybar config

from https://github.com/adi1090x/polybar-themes

Installed fonts from https://github.com/ryanoasis/nerd-fonts



