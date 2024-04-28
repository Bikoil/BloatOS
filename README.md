# Welcome to BloatOS Documentation!
I will be showing you how I was able to bloat ubuntu into an oblivion


***

# ⚠️ WARNING
- *PLEASE BE CAUTIOUS IF FOLLOWING THE DOCUMENTED STEPS, YOU MAY RUN INTO MULTIPLE ISSUES DURING INSTALL, THIS IS NOT MEANT TO BE*


***

- At first, I got a Ubuntu Desktop ISO from [here](https://ubuntu.com/download/desktop) and then booted it up in a VM, then installed the following:

# Desktop Environments
- ___KDE Plasma___


  - For KDE desktop, I installed `kubuntu-desktop` from apt and made sure to not miss a single app that KDE offers, you can do this by doing:
```bash
sudo apt install kubuntu-desktop
```

- ___XFCE___


  - Now after installing KDE, I installed `xfce4` which was quite faster than KDE (due to its lightweightness, but hey who cares we want BLOAT!)
```bash
sudo apt install xfce4
```

- ___LXDE___


  - `lxde`, like XFCE is pretty light (It's in the name, duh) so it took a pretty short time to install
```bash
sudo apt install lxde
```

- ___LXQT___


  - `lxqt` like the other previously installed DE's was pretty easy to install (there is literally lightweight in the name)
```bash
sudo apt install lxqt
```

- ___DDE (Snap)___
  - `deepin-dde` is available for install in `snap` but in apt it's not available by default, you could go to [this article](https://itsfoss.com/install-deepin-ubuntu/) if you want the apt version
```bash
sudo snap install --edge deepin-dde --devmode
```
Do note that DDE is not installable without these flags, and [snap store](https://snapcraft.io/install/deepin-dde/ubuntu) does not mention that


- ___Cinnamon___
  - `cinnamon` was pretty easy to install like the other DE's
```bash
sudo apt install cinnamon
```

- ___MATE___
  - for `mate` I honestly expected it to be lightweight like XFCE or LXQT, but it was actually a bit heavier
```bash
sudo apt install mate
```


- ___Budgie___
  - budgie is one of the kinda heavy DE's, which was perfect for this OS
```bash
sudo apt install ubuntu-budgie-desktop
```


Now all DE's have been installed

*BUT WAIT, There is MORE!*
# Window Managers
Now that we have created an absolute abomination, why not double-down with WMs?

For this, i only installed 3 WMs, Sway, AwesomeWM and Dwm, this is because most WMs are already VERY lightweight

- ___AwesomeWM___

  - `awesome` was probably one of the fastest installs of them all
```bash
sudo apt install awesome
```

- ___Sway___
  - `sway`, like Awesome, was pretty fast to install
```bash
sudo apt install sway
```

- ___Dwm___
  - `dwm` like the other wms was easy to install
```bash
sudo apt install dwm
```

***




Okay, DE's and WMs have been installed and the applications are absolutely flooded with uselessness, Now let's move on into applications.

# Applications

- ___Flatpak___
  - `flatpak` will be a very essential role in bloating this system along with snap (which was pre-installed with ubuntu
```bash
sudo apt install flatpak
```

- ___Useless software___
  - For the useless software I started with `opera`, everyone's favourite eh? no one uses opera in linux so this was perfect for bloat!
```bash
sudo snap install opera
```
  - Then, I was gonna install `discord` via `apt` but `snap` just made apt not work with that installation, so I just used snap
```bash
sudo snap install discord
```
  - Now for wine, I used apt to install `wine64`, which was very easy
```bash
sudo apt install wine64
```
  - I also installed `krita` because it just fit with the collection of useless apps, I also added `gimp` and `audacity` to the mix of editing apps
```bash
sudo apt install krita gimp audacity
```
  - Then I added neofetch because like... pretty system info!!!
```bash
sudo apt install neofetch
```

- ___Text Editors___
  - Like DE's, no one agrees which Text editor is the best, so i installed most of the popular ones
  - I started with VScode, i couldnt use apt (because snap was being dumb) so i had to use snap
```bash
sudo apt install code --classic
```
  - then I went for the other popular text editors in apt
```bash
sudo apt install micro vim emacs ed kakoune
```

- ___Shells___
  - No one agrees which shell is the best, so i installed most of the popular ones (again lol)
```bash
sudo apt install fish ksh zsh
```

At this point your neofetch should look like this






![image](https://github.com/Bikoil/BloatOS/assets/139659047/16efc414-b38d-4946-a50c-191d09fe399d)



*I will continue to update this wiki to keep bloating ubuntu, this is how far i have gotten*


Here is the Script to bloat ubuntu
```bash
echo "WARNING: USE THIS AT YOUR OWN RISK"
# Please update APT before running this script, remember to run this as root
# kde installation
apt install kubuntu-desktop
# xfce installation
apt install xfce4
# lxde installation
apt install lxde
# lxqt installation
apt install lxqt
# dde (snap version) installation
snap install --edge deepin-dde --devmode
# cinnamon installation
apt install cinnamon
# mate installation
apt install mate
# budgie installation
apt install ubuntu-budgie-desktop
# awesome installation
apt install awesome
# sway installation
apt install sway
# dwm installation
apt install dwm


# flatpak installation
apt install flatpak
# opera installation
snap install opera
# discord installation
snap install discord
# wine installation
apt install wine64
# krita, gimp and audacity installation
apt install krita audacity gimp
# neofetch installation
apt install neofetch
# ide installations
apt install micro vim emacs ed kakoune
snap install code
# shell installation
apt install fish ksh zsh
echo "Congratulations, Your system is now Bloated!"
```
# Fork starts

## Development bloats
```bash
sudo apt install build-essential meson wget build-essential ninja-build cmake-extras cmake gettext gettext-base fontconfig libfontconfig-dev libffi-dev libxml2-dev libdrm-dev libxkbcommon-x11-dev libxkbregistry-dev libxkbcommon-dev libpixman-1-dev libudev-dev libseat-dev seatd libxcb-dri3-dev libegl-dev libgles2 libegl1-mesa-dev glslang-tools libinput-bin libinput-dev libxcb-composite0-dev libavutil-dev libavcodec-dev libavformat-dev libxcb-ewmh2 libxcb-ewmh-dev libxcb-present-dev libxcb-icccm4-dev libxcb-render-util0-dev libxcb-res0-dev libxcb-xinput-dev xdg-desktop-portal-wlr libtomlplusplus3 clang
```

## Other stuff
```bash
sudo apt install 0ad supertuxkart firefox-esr 
```
