---
tags:
  - "#hyprland"
  - "#help-guide"
Created On: 10-12-2024 09:12
URL: https://www.reddit.com/r/hyprland/comments/1auj2u6/comment/kr4loru/
---
# Changing default browser in hyprland


To get the current default web browser:

`xdg-settings get default-web-browser`

To set the default web browser:

`xdg-settings set default-web-browser firefox.desktop`

Obviously change Firefox to whatever browser you want, and remember that you have to point to the .desktop file of the browser

For more info, check [xdg-utils](https://wiki.archlinux.org/title/Xdg-utils)

