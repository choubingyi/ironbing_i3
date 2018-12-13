Introduction
===
IronBing's i3 windows manager config.
![screenshot](https://imgur.com/uQJXB1a)

Enable touchpad function for tap of click.
===
1. Check out the xinput command. xinput list will give you a list of input devices; 
2. find the ID of the one which looks like a touchpad. 
3. Then do xinput list-props <device id>, which should tell you what properties you can change for the input device. You should find one called something like Tapping Enabled and a number in parens after it (in my case, it's libinput Tapping Enabled (276). 
4. Finally, run xinput set-prop <device id> <property id> 1, and tapping should work.
