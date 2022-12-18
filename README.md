# My Linux Doc's 

## Warning 
- This is work in progress as I am still learning the i3 + polybar way on Arch.

## Arcolinux repo needed I guess:
```Terminal
sudo pacman -S alacritty nano arcolinux-i3wm-git archlinux-logout-git arcolinux-polybar-git archlinux-wallpapers-git autotiling dmenu feh i3blocks i3-gaps i3status picom polkit-gnome polybar thunar thunar-archive-plugin thunar-volman ttf-hack

```
##  default configs location?
- ~/.config/i3/config
- ~/.config/polybar/config

## Default keys
- fullscreen mod+f
- mod+arrow (move around focus i guess?)
- Shift + mod + arrow (move windows)
- Shift + mod + space (floating/tiling toggle?)
- Shift + mouse (move floating window 1 guess)
- mod + shift + 1/2 (move windows on other displays?)

## Feh
```
feh --bg-scale --zoom fill /usr/share/backgrounds/archlinux-login-backgrounds/att-01.jpg
```
### Config place tmp ? 
1. place bg from term
```
feh --bg-scale --zoom fill /home/stefan/Pictures/wallpaper.jpg
```
3. add to config i3wm
```
~/.fehbg
```
## i3 Cheat sheet
```
    startx i3 start i3 from command line.
    $mod+<Enter> open a terminal.
    $mod+d open dmenu (text based program launcher)
    $mod+r resize mode ( or to leave resize mode)
    $mod+shift+e exit i3.
    $mod+shift+r restart i3 inplace.
    $mod+shift+c reload config file.
```
## Wifi
```
nmcli dev wifi
nmcli device wifi connect ImeNaWifi password password
```
## Linux app live in (.desktop)
```
/usr/share/applications
```

## My fav apps
- micro (golang)
- tldr

## Keyboard layout (doesnt work with i3 config some bad bug)
Terminal command for changeing the layout
```
//Macedonian
setxkbmap mk
//English
setxkbmap us
```
# xrandr (VGA mode)
```
xrandr --output DP-1 --mode 1920x1080 --right-of eDP-1
```
### Other
```
xrandr --query
```
```
xrandr --listmonitors
xrandr --listactivemonitors
xrandr --listproviders
```

# Network
```
ip -f inet addr show wlan0
```

# Bluetooth
```
sudo /usr/lib/bluetooth/bluetoothd -n -d
```
# Curl download file
Tux example svg:
```
curl https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg -o tux.svg
```
