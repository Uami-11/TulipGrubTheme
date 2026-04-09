# Omniscient Reader's Viewpoint Grub Theme

<img width="1920" height="1080" alt="GRUB(1)" src="https://github.com/user-attachments/assets/a5073c46-02dd-40a6-9ec3-afc923f8c7e6" />

# Installation
```bash
git clone --depth=1 https://github.com/Uami-11/TulipGrubTheme && cd TulipGrubTheme && ./install.sh
```

### Manual installation
1. Clone this repo:
```bash
git clone --depth=1 https://github.com/Uami-11/TulipGrubTheme.git
cd TulipGrubTheme
```
2. Copy ```orv/``` into ```/boot/grub/themes/```:
```bash
sudo cp -rf orv /boot/grub/themes/
```
3. In ```/etc/default/grub```, uncomment the line that says "GRUB_THEME" and add the path to ```theme.txt```:
```bash
sudoedit /etc/default/grub

    # It should look like this:
    GRUB_THEME="/boot/grub/themes/orv/theme.txt"
```
4. Set ```GRUB_GFXMODE=``` to the correct resolution:
```bash
GRUB_GFXMODE=1920x1080 # in my case 1920x1080,auto which is also whats in install.sh
```
5. Optionally, make Grub remember the last option selected by modifying ```GRUB_DEFAULT=``` and ```GRUB_SAVEDEFAULT=```:
```bash
GRUB_DEFAULT=saved
GRUB_SAVEDEFAULT=true # Make sure to uncomment this one.
```

# Customizing
There is a quick guide on how to customize this theme further in the [wiki](https://github.com/uiriansan/LainGrubTheme/wiki/Customizing)

# Credits
Check out [uiriansan](https://github.com/uiriansan/LainGrubTheme)! Star them, they are very awesome

Wallpaper from [WallpaperAccess](https://wallpaperaccess.com/omniscient-readers-viewpoint), if you want other cool orv wallpapers, you can check it out there. And you can plop it in orv/assets/ and overwrite orv.png!
