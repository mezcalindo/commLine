### Boot to command line, and reveal modules loaded during that process
#### Manjaro (Arch Linux)
In order to configure a manjaro desktop such that:
1. it reveals what is being loaded, line by line, during boot
2. boots to a command line, as opposed to a graphical login screen

...the grub config file must be edited as follows:

1. Launch a terminal window.
2. Open the grub config file by issuing: ```sudo nano /etc/default/grub```
3. Arrow to the following line in the file: ```GRUB_CMDLINE_LINUX_DEFAULT="..."```
4. Delete the word ```quiet```
5. Add a ``` ``` (space) and a ```3``` after the ```UUID``` string
6. Key **_ctrl + o (^o)_** and confirm to write the file
7. Key **_ctrl + x (^x)_** to exit nano and return to the command line
8. Issue ```sudo update-grub```
9. Upon completion of grub config generation, may restart the machine to finalize the process (may issue ```shutdown -r now```)
