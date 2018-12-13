Introduction
===
IronBing's i3 windows manager config.
![screenshot](https://i.imgur.com/uQJXB1a.png)
**Window block information**
1. ***G+*** Chrome browser
2. ***Terminal*** Gnome-Terminal
3. ***Communication*** Line, Pidgin
4. ***nautilus*** Nautilus
5. ***Mail*** Evolution
6. ***Virtualbox*** Virtualbox
7. ***No Definition***
8. ***No Definition***
9. ***Translation*** StarDict
10. ***Connecter*** Bluetooth

More tools you need
===
***1. Enable touchpad function for tap of click.*** [1]
1. Check out the xinput command. xinput list will give you a list of input devices; 
2. find the ID of the one which looks like a touchpad. 
3. Then do xinput list-props <device id>, which should tell you what properties you can change for the input device. You should find one called something like Tapping Enabled and a number in parens after it (in my case, it's libinput Tapping Enabled (276). 
4. Finally, run xinput set-prop <device id> <property id> 1, and tapping should work.

Reference
===
[1] https://www.reddit.com/r/i3wm/comments/516e8c/tap_to_click_touchpad/
