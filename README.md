* Step to Install Debian VM using Virtual Box

```
Name : agavrel
Type : Linux
Version : Debian 64 bits
Memory Size : 1024
Create a Virtual Hard Disk now
VDI
Dynamically allocated
File location and storage: Storage-> Goinfre -> 42 username

```

Once created, you will need to download Debian from the official site:
https://cdimage.debian.org/debian-cd/current/i386/iso-cd/ -> download debian-9.3.0-i386-netinst.iso

Then start the newly created VM ('agavrel' in this example) and proceed with the Debian installation:
```
Settings -> Storage -> Controller IDE -> choose debian image and check Live CD/DVD
Then Start the VM and follow steps, always select default settings except for :
username : agavrel42
password : root
Partitions Disk -> choose yes
Software selection -> Add 'KDE' and 'SSH'
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
