# dwm

This is suckless, mmmbud, the source code is the documentation! Check out config.h.

Patches and features
Clickable statusbar with my build of dwmblocks.
Reads xresources colors/variables (i.e. works with pywal, etc.).
scratchpad: Accessible with mod+shift+enter.
New layouts: bstack, fibonacci, deck, centered master and more. All bound to keys super+(shift+)t/y/u/i.
True fullscreen (super+f) and prevents focus shifting.
stacker: Move windows up the stack manually (super-K/J).
shiftview: Cycle through tags (super+g/;).
vanitygaps: Gaps allowed across all layouts.
swallow patch: if a program run from a terminal would make it inoperable, it temporarily takes its place to save space.
gridmode (adding a grid layout)
My dwm config

Dependencies

libxft
ttf-joypixels
st
dmenu
Also, you will need to add the following from the AUR:
https://aur.archlinux.org/packages/libxft-bgra-git/ (needed for colored fonts and emojis)

Installing dwm
cd dwm
sudo make clean install

Running dwm

If you do not use a login manager (such as lightdm) then you can add the following line to your .xinitrc to start dwm using startx:
exec dwm

If you use a login manager (like lightdm), make sure that you have a file called dwm.desktop in your /usr/share/xsessions/ directory.  It should look something like this:
[Desktop Entry]
Encoding=UTF-8
Name=Dwm
Comment=Dynamic window manager
Exec=dwm
Icon=dwm
Type=XSession


