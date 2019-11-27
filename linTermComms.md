**_sudo add-apt-repository <repository name>_** :: add a repository so that you can install a program that is not available for install through your existing repositories. for example, the package libimobiledevice requires the ppa:mniess/libimobiledevice repository.

**_sudo apt-get purge <program name>_** :: purge/delete an installed program from your system.

**_ls -al_** :: list/show all files in a directory, including hidden files.

**_lsblk -f_** :: list all drives with partitions in tree format. output includes file types, identifiers, labels, serial numbers, and mount points.

**_mkfs.???_** :: make a filesystem on a drive. for instance, ```sudo mkfs.exfat /dev/sdb1```.

**_program name &_** :: launch a program (no quotes).

**_ps a_** :: see all running processes.

**_rm -rf <directory name>_** :: recursively remove/delete a directory and its contents. works for hidden directories as well, simply include the "." before the directory name.

**_rm <filename>_** :: remove/delete a single file.
  
**_sudo -i_** :: use terminal as system root user. for example, may need to issue this, followed by nautilus, in order to launch the file browser and be able to copy over files from a system to an external hard drive while a live boot environment so that you can bypass errors of the kind, "cannot read permissions".

**_sudo -s_** :: establish root access as user in terminal.

**_shutdown -h now_** :: shutdown machine without saving any OS session data.

**_shutdown -r now_** :: restart machine.

**_uname -a_** :: get info like your computer name and the version and architecture of your linux kernel.

**_yaourt -Syu --aur_** :: update all AUR packages in Manjaro.
