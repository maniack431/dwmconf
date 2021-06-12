# dwmconf
**My dwm dotfiles..:D**

**Requirements:**

   **_ARCH_**
   
    sudo pacman -Sy xorg xorg-xinit xorg-xserver network-manager-applet rxvt-unicode nitrogen acpi
    yay -Sy picom pnmixer ttf-font-awesome-4 ttf-dejavu flat-remix-gtk
 
 **Installation**
 1. Place .Xresources and .xinitrc in your $HOME directory 
 
        cd ~/dwmconf/ && cp .Xresouces ~/.Xresources && cp .xinitrc ~/.xinitrc
 2. Build the Window Manager
        
        cd ~/dwmconf/suckless/dwm && sudo cp config.def.h config.h && sudo make clean install && cd
 3. Build the Bar       
  
        cd ~/dwmconf/suckless/dwmblocks && sudo cp blocks.def.h blocks.h && sudo make clean install && cd
 4. Build the Run Prompt
 
        cd ~/dwmconf/suckless/dmenu && sudo cp config.def.h config.h && sudo make clean install && cd
 5. Build the Screen Lock
         
        cd ~/dwmconf/suckless/slockcustom/slock && sudo cp config.def.h config.h && sudo make clean install && cd
 
 Thank You and Have a Good Day :)
