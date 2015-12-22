# XFCE4 Bing Wallpaper
##### Set [Bing](http://bing.com) image as your Linux wallpaper.
***
I like Bing images for my wallpaper. On Windows you can use 'Bing Desktop' application to set your daily wallpaper from bing but there is no such thing on Linux.

## Requirements
This script is written in python 3 so all you need is a version 3 of python with no external libraries. Also this script is for [XFCE](http://www.xfce.org) DE, but you can make this suitable for [GNOME](http://www.gnome.org) or other environments as well by changing the command in line 49 for the corresponding DE.

## Usage
All you need to do is running this command:
```shell
    python script.py
```
You can run this script on system startup to change your wallpaper on boot. Locale can be changed too from 'hpimagearchive_url' field.

## Potential Issues
You may not succeed in changing your wallpaper so if image was download but your wallpaper did not change first run:
```shell
    xfconf-query -c xfce4-desktop -p /backdrop -m
```
Then try to change your wallpaper through normal desktop settings and see the result on terminal. Substitute the command in line 49 with what you see on terminal for proper result.
