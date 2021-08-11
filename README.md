# My Dotfiles ![Distribution](https://img.shields.io/badge/Distribution-Arch-blue)




## Installation
This setup requires a few programs to be installed
### Main
| Software | Description | Installation |
| --- | --- | --- |
| i3-gaps | Window manager | `sudo pacman -S i3-gaps` |
| feh | Set wallpapers | `sudo pacman -S feh` |
| rofi | Application launcher | `sudo pacman -S rofi` |
| pywal | Palette generator | `sudo pacman -S python-pywal` |
| Kitty | Terminal emulator | `sudo pacman -S kitty` |
| yay | AUR package manager | [Instructions here](https://github.com/Jguer/yay) |
| polybar | Status bar| `yay -S polybar` |
| picom | Window transparency | `yay -S picom` |

### Other
| Software | Description | Installation |
| --- | --- | --- |
| oh my zsh | zsh themes | `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"` 
| playerctl | Prerequisite for Spotify module in status bar | `sudo pacman -S playerctl` |
| zscroll | Prerequisite for Spotify module in status bar | `yay -S zscroll` |

After, paste the files from the config folder to `~/.config` and install the required fonts (below)

### Fonts
Required for polybar modules to work. After installing, execute `sudo fc-cache` to refresh fonts.
| Font | Installation |
| --- | --- |
| Font Awesome | `yay -S otf-font-awesome ttf-font-awesome` |
| Font Awesome 5 Free | `yay -S otf-font-awesome-5-free` |
| Iosevka Nerd | `yay -S ttf-iosevka` |
| Noto Sans CJK | `yay -S noto-fonts-cjk` |
| FiraCode Nerd | `yay -S nerd-fonts-fira-code` |
| Powerline | `sudo pacman -S powerline-fonts` |



## Additional Setup
- Window opacities can be changed in the `~/.config/picom.conf` file
- The wallpaper (with pywal palettes) can be changed through adding the image path to the `i3` config file. 
  - Alternatively, a `wal-scale` command is included in the `.zshrc` file that sets a wallpaper and generates a palette using pywal, but will reset to the config defaults upon refresh
- zsh theme can be changed through editing `ZSH_THEME` in the `.zshrc` config
	- Paste `refined-alt.zsh-theme` in `~.oh-my-zsh/themes` and **change the name on line 40**  
 > Make all .sh files executable using `chmod u+x [file].sh` 

## Additional Software
| Software | Description | Installation |
| --- | --- | --- |
| cli-visualiser | Music visualiser | `sudo pacman -S ncurses fftw cmake`
| pokemon-colorscripts  | Pokemon sprites in terminal | [Instructions here](https://gitlab.com/phoneybadger/pokemon-colorscripts) |
| neofetch | Device statistics| `sudo pacman -S neofetch` |
| ranger | File manager | `sudo pacman -S ranger` |

## Todo
 - [ ] Setup Betterdiscord with pywal
 - [ ] Setup Spicetify with pywal
 - [ ] Setup Firefox with pywal
 - [ ] Setup cli-visualiser
 - [x] Setup pokemon-colorscripts to run on terminal launch
 - [ ] Setup neofetch config
 - [ ] Setup rofi theme
