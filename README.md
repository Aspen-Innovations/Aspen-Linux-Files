#Aspen-Linux
This is the official Aspen Linux Repository

Thank you for having the time for reading this, now, where should we start?

Booting the "boot.img" file:
(you can download it by the google drive link listed below)
https://drive.google.com/drive/folders/1kXq32pg1fIY7f_6IMKOUcyauZFw8obzT?usp=drive_link
If you want to boot it (on linux), i recommend you use qemu with this command: "qemu-system-x86_64 -m 8096 -vga cirrus boot.img" You are COMPLETELY FREE to find out other methods of booting it, hell, i'll personally nominate you if you do. You are also free to modify/poke around in the boot.img file, but please credit us for the original content.

Downloading the individual files and putting them into a .img file
The files are stored externally (to save space) here: [Download Large Files from Google Drive](https://drive.google.com/drive/folders/1kXq32pg1fIY7f_6IMKOUcyauZFw8obzT?usp=drive_link)
There is a method i use, where i put contents of Aspen Linux (listed below) in a folder, make a ".img" file, mount it to an empty folder, copy the contents of the distro to the empty folder that the .img is mounted to, unmounting it, and booting it via qemu.

WARNING: I am YET TO ADD user accounts, (since i'm too tired). I will add that later.
In order to do this, you need to download the folders and files listed below:

bin, boot, etc, lib, lib64, opt, sbin, tmp, usr, var, bzImage, linuxrc, profile.
then use the method already listed above.

BE AWARE, THIS METHOD IS NOT ALWAYS RELIABLE!

Contact us at "softwaredeveloper@aspen-innovations.org" for support on this method. psst, the "profile" file is the one that runs the welcome text on boot, as well as the many aliases for the many commands.
