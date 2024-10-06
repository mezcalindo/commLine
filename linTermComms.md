**_./_** :: indicates the working directory.

**_sudo add-apt-repository <repository name>_** :: add a repository so that you can install a program that is not available for install through your existing repositories. for example, the package libimobiledevice requires the ppa:mniess/libimobiledevice repository.

**_sudo apt-get purge <program name>_** :: purge/delete an installed program from your system.
  
**_cat /etc/issue_** :: identify linux distro name and version number.

**_cat /etc/*release_** :: identify linux distro and version, expanded information.

**_eject /dev/sr0_** :: eject a disk (CD, DVD).

**_fsck /dev/sd[xy]_** :: check a filesystem on a drive for errors.

**_ls -al_** :: list/show all files in a directory, including hidden files.

**_lsblk -f_** :: list all drives with partitions in tree format. output includes file types, identifiers, labels, serial numbers, and mount points.

**_lsb_release -a_** :: print the version of the linux distro running on the system.

**_mkfs.???_** :: make a filesystem on a drive. for instance, ```sudo mkfs.exfat /dev/sdb1```.

**_sudo nano /etc/default/grub_** :: edit the grub config file utilizing nano in the terminal window.

**_sudo pacman -Qdt_** or **_sudo pacman -Qdtq_** :: list orphaned packages.

**_sudo pacman -Rsn package-name_** :: remove any package and all dependencies and configuration file modifications. Otherwise, to focus on just the package, utilize **_sudo pacman -R package-name_**.

**_sudo pacman -S archlinux-keyring_** :: update the keyring while troubleshooting pacman update issues.
  
**_sudo pacman -Sc_** :: purge the pacman cache.
  
**_sudo pacman -Syyu_** :: update all databases and packages on manjaro, not including those from the AUR.

**_sudo pacman -Syyu --debug_** :: debug the pacman update process.
  
**_pamac clean --build-files_** :: clean out any files that were used for building packages previously. part of system maintenance.

**_pamac remove --orphans_** :: remove orphaned files.
  
**_pamac upgrade -a_** :: update all packages on manjaro, including those from the AUR. Note, don't precede the command with **_sudo_**; the system will make a request for elevated privileges if necessary.

**_program name &_** :: launch a program (no quotes).

**_ps a_** :: see all running processes.

**_rm -rf <directory name>_** :: recursively remove/delete a directory and its contents. works for hidden directories as well, simply include the "." before the directory name.

**_rm <filename>_** :: remove/delete a single file.

**_sudo snap refresh_** :: manually check for updates to installed snaps.

**_sudo snap remove package-name_** :: remove a particular snap install.

**_snap info package-name_** :: get detailed info on an installed snap.
  
**_sudo -i_** :: use terminal as system root user. for example, may need to issue this, followed by nautilus, in order to launch the file browser and be able to copy over files from a system to an external hard drive while a live boot environment so that you can bypass errors of the kind, "cannot read permissions".

**_sudo -s_** :: establish root access as user in terminal.

**_shutdown -h now_** :: shutdown machine without saving any OS session data.

**_shutdown -r now_** :: restart machine.

**_systemctl enable service-name_** :: enable a particular service. for instance, ```systemctl enable cups```.

**_systemctl is-enabled service-name_** :: is the service enabled? for instance, ```systemctl is-enabled cups```.

**_systemctl start service-name_** :: start a particular service. for instance, ```systemctl start cups```.

**_systemctl status service-name_** :: check the status of a particular service. for instance, ```systemctl status cups```.

**_uname -a_** :: get info like your computer name and the version and architecture of your linux kernel.

**_sudo update-grub_** :: force grub to reload.

**_xfce4-session-logout --logout_** :: log out of the xfce desktop.

**_xfdesktop -R_** :: restart the Xfce desktop (arch linux, manjaro, etc).

**_yaourt -Syyu --aur_** :: update all AUR packages in Manjaro.
  
**_yay -Syyu_** :: update all packages, including those from the AUR, in Manjaro.
  
**_yay -S package-name_** :: update a single specific package. be sure to update package databases first.

**_yay -Qii package-name_** :: check various details of a package, including dependencies.
