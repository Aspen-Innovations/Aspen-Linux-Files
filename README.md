# Aspen-Linux
This is the official Aspen Linux Repository

Thank you for having the time for reading this, now, where should we start?

Booting the "boot.img" file:
(you can download the boot.img by the google drive link listed below)
https://drive.google.com/file/d/1memeJpZePz841H-qNmAr74K0aRSBRbkn/view?usp=drive_link
If you want to boot it (on linux), 
I recommend you use qemu with this command: "qemu-system-x86_64 -m 8096 -vga cirrus boot.img" You are COMPLETELY FREE to find out other methods of booting it, hell, i'll personally nominate you if you do. You are also free to modify/poke around in the boot.img file, but please credit us for the original content.

**THIS METHOD IS FOR LINUX USERS:**
# Downloading the individual files and putting them into a .img file:
The files are stored externally (to save space) here: [Download Large Files from Google Drive](https://drive.google.com/drive/folders/1kXq32pg1fIY7f_6IMKOUcyauZFw8obzT?usp=drive_link)

**Put all the contents of Aspen Linux into a folder (let’s call it Aspen_Folder).**

Make an empty .img file (this is where the system will be installed).
Use the following command to create a blank image (for example, 2GB in size):
```dd if=/dev/zero of=aspen.img bs=1M count=2048```

**Mount the .img File**

Create an empty folder to mount the .img file (e.g., mount_point).
```mkdir mount_point```
Mount the .img file to that folder:
```sudo mount -o loop aspen.img mount_point```

**Copy Files from Aspen Linux**

Copy the contents of your Aspen Linux folder (Aspen_Folder) to the mounted folder:
```cp -r Aspen_Folder/* mount_point/```

**Unmount the .img File**

After the copy is done, unmount the .img file:
```sudo umount mount_point```

**Boot with QEMU:**

Now you’re ready to boot the system via QEMU. Run this command:
```qemu-system-x86_64 -drive file=aspen.img,format=raw```

That’s it! You’ve just set up and booted Aspen Linux in QEMU.
Now, I have NOT figured out how to do this on windows, you're on your own with that one.

WARNING: I am YET TO ADD user accounts, (since i'm too tired). I will add that later.
In order to do this, you need to download the folders and files listed below:

bin, boot, etc, lib, lib64, opt, sbin, tmp, usr, var, bzImage, linuxrc, profile.
then use the method already listed above.

BE AWARE, THIS METHOD IS NOT ALWAYS RELIABLE!

Contact us at "softwaredeveloper@aspen-innovations.org" for support on this method. 
psst, the "profile" file is the one that runs the welcome text on boot, as well as the many aliases for the many commands.
