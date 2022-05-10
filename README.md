# i3_install_guide
I will save here my install and config of Arch linux

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

alternative:
  add to ~/.zshrc << setxkbmap es

## copy i3/config in ~/.config


## polybar config

from https://github.com/adi1090x/polybar-themes

Installed fonts from https://github.com/ryanoasis/nerd-fonts

to fix rofi weird aspect:
```
find ~/ -name '*.rasi' | xargs sed -i "s/element-text\s*{$/element-text {\n    background-color:  @al;\n    text-color: inherit;\n/g"
´´´
and
´´´
find ~/ -name '*.rasi' | xargs sed -i "s/element-icon\s*{$/element-icon {\n    background-color:  @al;\n    text-color: inherit;\n/g" 
´´


