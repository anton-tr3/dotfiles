# My Dotfiles



## Installation
This setup requires a few programs to be installed
### Main
| Software | Description | Installation |
| --- | --- | --- |
| i3-gaps | Window manager | `sudo pacman -S i3-gaps` |
| polybar | Status bar| `sudo pacman -S polybar` |
| neofetch | Device statistics| `sudo pacman -S neofetch` |
| feh | Set wallpapers | `sudo pacman -S feh` |
| yay | AUR package manager | [Instructions here](https://github.com/Jguer/yay) |
| picom | Window transparency | `yay -S picom` |

### Other
| Software | Description | Installation |
| --- | --- | --- |
| playerctl | Prerequisite for Spotify module in status bar | `sudo pacman -S playerctl` |
| zscroll | Prerequisite for Spotify module in status bar | `yay -S zscroll` |

After, paste the files from the config folder to `~/.config` and the fonts to `~/usr/share`


## Setup
- Window opacities can be changed in the `~/.config/picom.conf` file
- The wallpaper (with pywal palettes) can be altered through adding the image path to the `i3` config file. 
  - Alternatively, a `wal-scale` command is included in the `.zshrc` file that sets a wallpaper and generates a palette using pywal, but will reset to the config defaults upon refresh

## Additional Software
| Software | Description | Installation |
| --- | --- | --- |
| cli-visualiser | Music visualiser | `sudo pacman -S ncurses fftw cmake`
| pokemon-colorscripts  | Pokemon sprites in terminal | [Instructions here](https://gitlab.com/phoneybadger/pokemon-colorscripts) |

## Todo
 - [ ] Setup betterdiscord with pywal
 - [ ] Setup spicetify with pywal
 - [ ] Setup 
