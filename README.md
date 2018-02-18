* Step to Install Debian VM using Virtual Box

```
Name : agavrel
Type : Linux
Version : Debian 64 bits
Memory Size : 1024
Create a Virtual Hard Disk now
VDI
Dynamically allocated
File location and storage:
Storage/goinfre/42/username OR MacOS/sgoinfre/goinfre/Perso/username if you wish to have it on the network
```

Once created, you will need to download Debian from the official site:
https://cdimage.debian.org/debian-cd/current/i386/iso-cd/ -> download debian-9.3.0-i386-netinst.iso

Then start the newly created VM ('agavrel' in this example) and proceed with the Debian installation:
```
Settings -> Storage -> Controller IDE -> choose debian image and check Live CD/DVD
Then Start the VM and follow steps, always select default settings except for :
username : agavrel42
password : root
Partitions Disk -> choose yes at the very end
< ... you will have to wait like 3mn ... >
Software selection -> Add 'KDE' and 'SSH'
< ... you will have to wait like 5mn take a coffee ? ... >
Install GRUB boot loader -> select '/dev/sda' (default suggested disk)
```

Enter your password.
You can then launch the terminal by clicking at the bottom left of your session
Finally switch from user to root with:
```
su - root
```

* Misc
Whenever you look for a specific file just use:
```
find / -type f -name "specific_file" -print
```

If you want to copy paste from your OS to the VM or reversely :
```
To enable it, open VirtualBox and select the guest machine, then click the settings button or press Ctrl + S on your keyboard.
Next, on the General page, select Advanced tab and make sure bidirectional is selected for Shared Clipboard as well as Drag’n’Drop options.
```
