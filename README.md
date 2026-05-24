# Fallout limine theme
For v12 of Limine
<img width="3550" height="2012" alt="IMG_20260524_124058" src="https://github.com/user-attachments/assets/445803ae-422c-4a30-b07d-ad71bca69e68" />


## Installation

Note: This repo only contains additional theming elements and is not a replacement for Limine.conf. It is assumed that a working Limine bootloader is already set up.

### Download the packages:
```
git clone https://github.com/Neptune3013/fallout-limine-theme.git
```
### Copy files to Boot direcory:
NOTE: Make a snapshot beforehand in case you mess up.

The following requires Admin mode and assumes the boot directory is /boot.

- Copy background.png and PHXEGA8.F14 to Boot directory.
- Copy the contents of Limine.txt into the beginning of Limine.conf in Boot directory. (it is safer to make a backup of the original limine.conf)

### Edit Limine.conf
The following are specific to v12 of Limine (Last tested with v12.3)
#### If not using Secure Boot
Nothing to change. 

#### If Using Secure Boot
- Run `sudo b2sum /boot/background.png` and append the output followed by a "#" after `wallpaper: boot():/background.jpg` in Limine.conf
- Run `sudo b2sum /boot/PHXEGA8.F14` and append the output followed by a "#" after `term_font: boot():/PHXEGA8.F14` in Limine.conf

It should look something like this:
```
wallpaper: boot():/background.jpg#1654643541984165196841356181561+8463516846516

term_font: boot():/PHXEGA8.F14#164684651984685416849684165198646541651616168465
```
(DO NOT COPY THE SAMPLE HASH SHOWN HERE, generate your own as instructed above.)

If hash string is not added, Limine will switch to its default appearance.

Note: If using Secure boot and hash string is not appended to the ***boot options***, Limine will PANIC. So do not touch that part of Limine. This repo is only dealing with theming elements of Limine.

### Update Bootloader

Run `limine-update`
