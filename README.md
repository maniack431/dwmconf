# dwmconf
**My DWM dotfiles :D**

**Requirements:**

   **_ARCH_**
   
    sudo pacman -Sy xorg xorg-xinit xorg-xserver network-manager-applet rxvt-unicode nitrogen acpi lxappearance
    yay -Sy picom pnmixer ttf-font-awesome-4 ttf-dejavu flat-remix-gtk
    
   **_DEBIAN_**
   
    sudo apt-get install xorg x11-common xdg-utils xorg-dev nitrogen network-manager-gnome rxvt-unicode picom fonts-dejavu-core make
   _For installing Font Awesome Icons:_
   1. Download <a href=https://github.com/FortAwesome/Font-Awesome>this</a> zip
   2. Place the contents from the 'otfs' directory to your .fonts directoy
      
    mkdir .fonts && cp -r ~/Downloads/Font-Awesome-master/otfs/ ~/.fonts
   3. Reload the font cache 

    fc-cache -f -v
         
 **Installation:**
 1. Place .Xresources and .xinitrc in your $HOME directory 
 
        cd ~/dwmconf/ && cp .Xresources ~/.Xresources && cp .xinitrc ~/.xinitrc
 2. Build the Window Manager
        
        cd ~/dwmconf/suckless/dwm && sudo cp config.def.h config.h && sudo make clean install && cd
 3. Build the Bar       
  
        cd ~/dwmconf/suckless/dwmblocks && sudo cp blocks.def.h blocks.h && sudo make clean install && cd
 4. Build the Run Prompt
 
        cd ~/dwmconf/suckless/dmenu && sudo cp config.def.h config.h && sudo make clean install && cd
 5. Build the Screen Lock
         
        cd ~/dwmconf/suckless/slockcustom/slock && sudo cp config.def.h config.h && sudo make clean install && cd
        
    _To run the Screen Locker you have to run it using dmenu, just type "slock"_
 
 **Thank You and Have a Good Day :)**
