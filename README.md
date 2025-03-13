
# Description
This program allows to set up a wallpaper via sxiv on 2 or more monitors. 

# Dependencies 
## X11 variation
- sxiv 
- xargs 
- feh 

## Hyprland variation
- sxiv 
- hyprpaper

# Installation for Hyprland
0. `git clone https://AlGaRitm2020/wallp && cd wallp`
1. Install dependencies via your package manager. For instance, in Arch: `sudo pacman -S sxiv hyprpaper`
2. After installation, check your monitors names via `hyprctl monitors` and replace 'eDP-1' and 'DP-2' strings in file 'wallp_hypr' to your monitors names.  
3. Make config for sxiv for dark background: `cp .Xresourses_sample ~/.Xresources`. You can configure this file as you want later. 
4. Reload xresources via `xrdb -load ~/.Xresources`
5. Final step: coping walp to binaries. `sudo cp wallp_hypr /usr/local/bin/wallp`.

# Usage 
- enter `wallp` to launch
- navigate between images via arrows or "jkl;" (vim keybindings)
- mark image (images) to be your background via 'm'
- type 'q' for exit and wallpappers will be set up.  

# The future 
Now wallp chose from .config/hypr/wallpaper directory (you can directly change it), but later I'll add option to choose path in arguments. 
