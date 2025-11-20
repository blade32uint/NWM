Changes added to dwm; 
  autostart applied(autostart.sh should be placed in ~/local/share/dwm)
  fullgaps applied
  changed default refresh rate in dwm.c from 60hz to variable refrenced in (config.def.h)


Dependencies
------------

Arch
  sudo pacman -S base-devel libx11 libxft libxinerama freetype2 fontconfig

Debian
  sudo apt build-dep dwm

Fedora
  sudo dnf install libX11-devel libXft-devel libXinerama-devel

Void
  sudo xbps-install -S base-devel libX11-devel libXft-devel libXinerama-devel freetype-devel fontconfig-devel

OpenSUSE
  sudo zypper install git make gcc libX11-devel libXft-devel libXinerama-devel



Installation
------------
clone this repo to your home folder
  
  cd && git clone https://github.com/blade32uint/NWM

Change working directory to the DWM folder
  cd ~/DWM
  
Edit config.def.h (you can set refreshrate and gap size at the top)
  Change the font, gap size, refresh rate and keybinds to your preference.
  USE EDITOR OF CHOICE

Delete config.h file
  rm -r config.h (be carful not to delete the config.def.h that is your main config file.)

Building And Rebuilding After Changes
  rm -r config.h && make && make clean install








